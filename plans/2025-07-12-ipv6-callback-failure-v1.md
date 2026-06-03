# IPv6 Callback Failure Investigation

## Objective
Further investigate why _parse_pkt_in in IPV6SolicitationController is not called for RS packets, despite pipelined on controller ID 5 and rule matches, focusing on conditions, event dispatching, and configurations.

## Implementation Plan
1. **Analyze Callback Conditions**
  - Dependencies: None
  - Notes: Review early returns in code.
  - Files: ipv6_solicitation.py
  - Status: Not Started
2. **Check Event Registration**
  - Dependencies: Task 1
  - Notes: Examine handler setup.
  - Files: ipv6_solicitation.py, service_manager.py
  - Status: Not Started
3. **Update IPv6.md**
  - Dependencies: Task 2
  - Notes: Incorporate new reasons.
  - Files: IPv6.md
  - Status: Not Started

## Verification Criteria
- Identified specific condition or dispatch issue causing failure.
- Updated documentation with findings.
- Alignment with user log tests.

## Potential Risks and Mitigations
1. **Runtime Only Issues**
   Mitigation: Rely on user-provided logs.
2. **Config Dependencies**
   Mitigation: Ask for specific values.

## Alternative Approaches
1. Log Analysis: Guide user on adding more logs.
2. Code Tracing: Simulate flow without changes.