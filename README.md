# SIEM Microsoft Sentinel Project
Ingesting logs from a Honeypot VM setup within Azure to examine traffic location for failed RDP attempts

## Network Topology
![topology](https://github.com/DRDohvaken/siem-azure-project/assets/8603276/f6e9668c-88ae-4b9b-b2ba-691f10502226)

- Honey-VM-vnet - Virtual Network
- default - Subnet
- honeypot-vm-win808 - Network Interface
- Honeypot-VM-WIN - Virtual Machine
- Honeypot-VM-WIN-nsg - Network security group
- Honeypot-VM-WIN-ip - Public IP address
