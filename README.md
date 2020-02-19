# Ansible-Demo
 General NetApp Ansible integration demonstration

# This repo is for sharing a standardizing set of Ansible demo files

# Top-level are Demo containers for Ansible playbooks for NetApp platforms.
Element - Contains a simple volume creation workflow

Requirements:
- Element OS Demo-node or similar

General ONTAP Demo - Is a 2 node configuration workflow, with a source and destination. This includes playbooks for configuration with both roles and modules, provisioning, SnapMirror replication, client access, and using ansible-vault.

Requirements:
- destination system (vsim)
- source system (vsim)

Note: Any ONTAP 9.3+ based system could be used with some adaptation: SimulateONTAP (vsim), ONTAP Select, etc.

Key Elements:
- Leverages a prompt for passwords
- Uses NetApp 'Roles' for cluster and Storage VM configuration
- Manages export-policies
- Basic non-Role SnapMirror setup

Updated playbooks for ansible 2.9 and collections.
