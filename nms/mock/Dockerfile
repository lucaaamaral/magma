# Copyright 2023 The Magma Authors.

# This source code is licensed under the BSD-style license found in the
# LICENSE file in the root directory of this source tree.

# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

FROM node:16.14-alpine AS builder

WORKDIR /usr/src/

# Copy project dependencies
COPY package.json yarn.lock babel.config.js ./

# Install node dependencies
RUN yarn install --mutex network --frozen-lockfile && yarn cache clean

# Build our static files
COPY . .

FROM node:16.14-alpine

# Install required binaries
RUN apk add ca-certificates curl bash
COPY wait-for-it.sh /usr/local/bin

COPY --from=builder /usr/src /usr/src

WORKDIR /usr/src
CMD ["yarn run mockserver"]
