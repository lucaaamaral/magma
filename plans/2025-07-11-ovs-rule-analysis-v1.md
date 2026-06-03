# IPv6 OVS Rule Interference Analysis

## Objective
To inspect ovs_rules.txt for rules interfering with router solicitation packets, preventing them from reaching the pipelined controller, and update IPv6.md with findings.

## Implementation Plan
1. **Inspect ovs_rules.txt**
  - Dependencies: None
  - Notes: Focus on table 3 and prior.
  - Files: `plans/ovs_rules.txt`
  - Status: Completed
2. **Diagnose Interference**
  - Dependencies: Step 1
  - Notes: Conceptual based on dump.
  - Files: `plans/ovs_rules.txt`
  - Status: Completed
3. **Update IPv6.md**
  - Dependencies: Step 2
  - Notes: No code changes.
  - Files: `/home/lucas/Documents/Github/magma/IPv6.md`
  - Status: Not Started

## Verification Criteria
- Identification of potential interfering rules.
- Updated IPv6.md with analysis.

## Potential Risks and Mitigations
1. **Missing Runtime Data**
   - Mitigation: Request additional packet metadata.

## Alternative Approaches
1. **Flow Simulation**: Suggest using ovs-appctl to trace packet.
