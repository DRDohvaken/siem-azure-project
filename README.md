# SIEM Microsoft Sentinel Project
Ingesting logs from a Honeypot VM setup within Azure to examine traffic location for failed RDP attempts

## Failed RDP attempts by Geolocation after 2 hours
![map](https://github.com/DRDohvaken/siem-azure-project/assets/8603276/fe3f5062-c547-479d-b181-d0a66596c3fe)

## Network Topology
![topology](https://github.com/DRDohvaken/siem-azure-project/assets/8603276/f6e9668c-88ae-4b9b-b2ba-691f10502226)

- Honey-VM-vnet - Virtual Network
- default - Subnet
- honeypot-vm-win808 - Network Interface
- Honeypot-VM-WIN - Virtual Machine
- Honeypot-VM-WIN-nsg - Network security group
- Honeypot-VM-WIN-ip - Public IP address

### Step 1 - Create VM which will be exposed to the Internet
### Step 2 - Allow all inbound traffic into the VM to fully expose it within a Network Security Group
### Step 3 - Enable Log Analytics Workspace and Microsoft Defender
### Step 4 - Connect Log Analytics Workspace to the VM
### Step 5 - Add Microsoft Sentinel (SIEM) to the Workspace
### Step 6 - Run Powershell script on the VM to capture custom logs (Geolocation of failed RDP attempts)
### Step 7 - Extract logs from VM and display location of failed RDP attempts
- Create a new Workbook within Microsoft Sentinel
- Use the query in the *query.txt* to extract needed information from the custom logs.

