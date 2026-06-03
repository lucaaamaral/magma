# IPv6 Solicitation Event Analysis

## Objective
To update IPv6.md with details on OFPPacketIn events, their function, the callback for router solicitation, and analysis of why a specific packet may not trigger the callback despite rule matching.

## Implementation Plan
1. **Analyze OFPPacketIn and Callback**
  - Dependencies: None
  - Notes: Conceptual only.
  - Files: `lte/gateway/python/magma/pipelined/app/ipv6_solicitation.py`
  - Status: Completed
2. **Diagnose Packet Issue**
  - Dependencies: Step 1
  - Notes: May need more details.
  - Files: User-provided packet info
  - Status: In Progress
3. **Update IPv6.md with Details**
  - Dependencies: Step 2
  - Notes: Highlight callback function.
  - Files: `/home/lucas/Documents/Github/magma/IPv6.md`
  - Status: Not Started

## Verification Criteria
- IPv6.md includes explanations of OFPPacketIn and callback.
- Analysis of packet issue added.
- No code modifications.

## Potential Risks and Mitigations
1. **Incomplete Diagnosis**
   - Mitigation: Ask for more packet details.
2. **Overly Technical Details**
   - Mitigation: Keep conceptual.

## Alternative Approaches
1. **Log-Based Analysis**: Suggest user reviews logs for event triggers.
2. **External Refs**: Add links to Ryu/OpenFlow docs.