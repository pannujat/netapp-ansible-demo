# NetApp Ansible Demo
 General NetApp Ansible integration demonstration

# This repo is for sharing a standardizing set of Ansible demo files

ONTAP Demo Requirements:
- 2 x vsims (ONTAP 9.7)
- - One primary or "source" cluster
- - One secondary or "destination" cluster
- - destination system (vsim)
- - source system (vsim)
- - install netapp.ontap collection

This demo includes plays for:
* configuration with both roles and modules
* * Uses NetApp 'Roles' for cluster and Storage VM configuration
* SnapMirror replication - using modules
* ansible-vault - password alternative

Key Elements:
- Leverages a prompt for passwords
- Manages export-policies
- (re)naming
- Addition standard install best practices


Setup Requirements:

ansible-galaxy collection install netapp.ontap (-p /usr/share/ansible/collections)

- Install the NetApp libraries:
--netapp-lib
--solidfire-sdk-python

Note: Any ONTAP 9.3+ based system could be used with some adaptation: SimulateONTAP (vsim), ONTAP Select, etc.
