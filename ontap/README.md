# NetApp Ansible Demo
## General NetApp Ansible integration demonstration

**ONTAP Demo Requirements:**
- 2 x vsims (ONTAP 9.7)
  - source system (vsim)
    - Primary or "source" cluster
  - destination system (vsim)
    - Secondary or "destination" cluster
- install netapp.ontap collection

This demo includes plays for:
* configuration with both roles and modules
  * Uses NetApp 'Roles' for cluster and Storage VM configuration
* SnapMirror replication - using module(s) not roles
* ansible-vault - password alternative

**Key Elements:**
- Leverages a prompt for passwords
- Manages export-policies
- (re)naming
- Addition standard install best practices


**Note:** Any ONTAP 9.3+ based system could be used with some adaptation: SimulateONTAP (vsim), ONTAP Select, etc.
