# Controller ID Investigation

## Objective
Investigate controller IDs in Magma pipelined, determine if _parse_pkt_in in IPV6SolicitationController is registered on ID 5, and identify all possible IDs for the service manager or controller, updating documentation accordingly.

## Implementation Plan
1. **Search for controller_id in Code**
  - Dependencies: None
  - Notes: Use fs_search to find references.
  - Files: lte/gateway/python/magma/pipelined/*.py
  - Status: Not Started
2. **Analyze Findings**
  - Dependencies: Task 1
  - Notes: Review for ID assignments and registrations.
  - Files: Relevant from search
  - Status: Not Started
3. **Update IPv6.md**
  - Dependencies: Task 2
  - Notes: Add ID investigation results.
  - Files: IPv6.md
  - Status: Not Started

## Verification Criteria
- Confirmed if _parse_pkt_in is on ID 5.
- Listed all possible IDs.
- Updated IPv6.md.

## Potential Risks and Mitigations
1. **Search Failures**
   Mitigation: Use proper file_pattern.
2. **Config Access**
   Mitigation: Ask user if needed.

## Alternative Approaches
1. User Provided Config: Directly ask for ID values.
2. Broader Search: Include config directories.