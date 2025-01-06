
![cloud-computing-azure-00](https://github.com/user-attachments/assets/f63556bf-408f-49ba-8022-ef1e760330a4)




# Azure Tutorial: Create a Resource Group, Virtual Network, and Virtual Machine
Description: This tutorial demonstrates how to create essential Azure resources:

A Resource Group to organize resources.
A Virtual Network (VNet) to enable private communication.
A Virtual Machine (VM) to run applications.
Demonstration Section
The demonstration section shows users how to use the project step by step. It includes clear instructions, visuals, and testing to ensure users can replicate the process.

1. Define the Goals of the Demonstration
Clearly outline what the user will achieve by following this section:

Create an Azure Resource Group.
Set up a Virtual Network with a subnet.
Deploy a Virtual Machine into the virtual network.
Connect to the Virtual Machine.
2. Step-by-Step Walkthrough with Screenshots
Each step should be accompanied by screenshots to make it easier for users to follow.

Step 1: Create a Resource Group
Log in to the Azure Portal.

Go to Resource Groups and click + Create.

Fill out the form:

Name: MyResourceGroup.
Region: Select the closest location.
Click Review + Create, then Create.

Screenshot: Show the filled-out form and the Resource Group overview.

Step 2: Create a Virtual Network
Navigate to Virtual Networks in the Azure Portal.

Click + Create.

Fill out the form:

Name: MyVirtualNetwork.
Address Space: 10.0.0.0/16.
Add a subnet:

Subnet Name: MySubnet.
Address Range: 10.0.1.0/24.
Click Review + Create, then Create.

Screenshot: Show the form and the Virtual Network overview.

Step 3: Deploy a Virtual Machine
Go to Virtual Machines and click + Create > Azure Virtual Machine.

Fill out the form:

Name: MyVirtualMachine.
Region: Same as the Resource Group.
Size: Standard_B1s.
Admin Username: azureuser.
Password: Create a secure password.
Under Networking, select:

Virtual Network: MyVirtualNetwork.
Subnet: MySubnet.
Click Review + Create, then Create.

Screenshot: Show the VM configuration and the successful deployment message.

Step 4: Connect to the Virtual Machine
Go to the Virtual Machine overview page in Azure.

Use the Connect option:

Windows VM: Download the RDP file and connect using Remote Desktop.
Linux VM: Use SSH to connect (ssh azureuser@<VM-IP>).
Verify the connection by running a test command:

For Windows: Open Command Prompt and run ipconfig.
For Linux: Run ls or any simple command.
Screenshot: Show the connected VM desktop or terminal output.

3. Test the Setup
Provide instructions for testing the deployed resources:

Ping the VM to test connectivity.
Verify the Virtual Network and Subnet by viewing their properties.
Demonstrate application hosting or additional functionality (if applicable).
Screenshot: Show the testing process, e.g., running commands inside the VM or viewing network logs.

4. Troubleshooting Section
Anticipate potential issues and provide solutions:

Issue: Cannot connect to the VM.
Solution: Ensure the NSG allows inbound RDP/SSH traffic.
Issue: Deployment errors.
Solution: Check quotas or permissions in the subscription.
README.md Example for the Demonstration Section
markdown
Copy code
## Demonstration

### Goal
This section guides you through:
- Creating an Azure Resource Group.
- Setting up a Virtual Network.
- Deploying a Virtual Machine into the network.
- Connecting to the Virtual Machine.

### Steps
1. **Create a Resource Group**:
   - Navigate to Resource Groups in the Azure Portal.
   - Click **+ Create**, fill out the details, and create the Resource Group.
   ![Create Resource Group]("C:\Users\TEMP.ANDREW\Desktop\Azure Project\images\az1.png")

2. **Set Up a Virtual Network**:
   - Go to Virtual Networks and click **+ Create**.
   - Add an address space and a subnet.
   ![Create Virtual Network](screenshots/create-virtual-network.png)

3. **Deploy a Virtual Machine**:
   - Navigate to Virtual Machines and click **+ Create**.
   - Configure the VM with an admin user, network, and size.
   ![Create Virtual Machine](screenshots/create-virtual-machine.png)

4. **Connect to the Virtual Machine**:
   - Use RDP (Windows) or SSH (Linux) to connect to the VM.
   ![VM Running](screenshots/vm-running.png)

### Testing
- Ping the Virtual Machine from your local system.
- Verify the IP address using `ipconfig` or `ifconfig` inside the VM.

### Troubleshooting
- **Connection Issues**: Ensure the Network Security Group allows RDP or SSH traffic.
- **Deployment Failures**: Check subscription quotas and region availability.




Azure-Resource-Group-VM-Tutorial/
├── README.md                 # Tutorial guide

├── screenshots/              # Images showing each step

│   ├── create-resource-group.png

│   ├── create-virtual-network.png

│   ├── create-virtual-machine.png

│   └── vm-running.png





Demonstration Section
The demonstration section shows users how to use the project step by step. It includes clear instructions, visuals, and testing to ensure users can replicate the process.

1. Define the Goals of the Demonstration
Clearly outline what the user will achieve by following this section:

Create an Azure Resource Group.
Set up a Virtual Network with a subnet.
Deploy a Virtual Machine into the virtual network.
Connect to the Virtual Machine.
2. Step-by-Step Walkthrough with Screenshots
Each step should be accompanied by screenshots to make it easier for users to follow.

Step 1: Create a Resource Group
Log in to the Azure Portal.

Go to Resource Groups and click + Create.

Fill out the form:

Name: MyResourceGroup.
Region: Select the closest location.
Click Review + Create, then Create.

Screenshot: Show the filled-out form and the Resource Group overview.

Step 2: Create a Virtual Network
Navigate to Virtual Networks in the Azure Portal.

Click + Create.

Fill out the form:

Name: MyVirtualNetwork.
Address Space: 10.0.0.0/16.
Add a subnet:

Subnet Name: MySubnet.
Address Range: 10.0.1.0/24.
Click Review + Create, then Create.

Screenshot: Show the form and the Virtual Network overview.

Step 3: Deploy a Virtual Machine
Go to Virtual Machines and click + Create > Azure Virtual Machine.

Fill out the form:

Name: MyVirtualMachine.
Region: Same as the Resource Group.
Size: Standard_B1s.
Admin Username: azureuser.
Password: Create a secure password.
Under Networking, select:

Virtual Network: MyVirtualNetwork.
Subnet: MySubnet.
Click Review + Create, then Create.

Screenshot: Show the VM configuration and the successful deployment message.

Step 4: Connect to the Virtual Machine
Go to the Virtual Machine overview page in Azure.

Use the Connect option:

Windows VM: Download the RDP file and connect using Remote Desktop.
Linux VM: Use SSH to connect (ssh azureuser@<VM-IP>).
Verify the connection by running a test command:

For Windows: Open Command Prompt and run ipconfig.
For Linux: Run ls or any simple command.
Screenshot: Show the connected VM desktop or terminal output.

3. Test the Setup
Provide instructions for testing the deployed resources:

Ping the VM to test connectivity.
Verify the Virtual Network and Subnet by viewing their properties.
Demonstrate application hosting or additional functionality (if applicable).
Screenshot: Show the testing process, e.g., running commands inside the VM or viewing network logs.

4. Troubleshooting Section
Anticipate potential issues and provide solutions:

Issue: Cannot connect to the VM.
Solution: Ensure the NSG allows inbound RDP/SSH traffic.
Issue: Deployment errors.
Solution: Check quotas or permissions in the subscription.
README.md Example for the Demonstration Section
markdown
Copy code
## Demonstration

### Goal
This section guides you through:
- Creating an Azure Resource Group.
- Setting up a Virtual Network.
- Deploying a Virtual Machine into the network.
- Connecting to the Virtual Machine.

### Steps
1. **Create a Resource Group**:
   - Navigate to Resource Groups in the Azure Portal.
   - Click **+ Create**, fill out the details, and create the Resource Group.
   ![Create Resource Group](screenshots/create-resource-group.png)

2. **Set Up a Virtual Network**:
   - Go to Virtual Networks and click **+ Create**.
   - Add an address space and a subnet.
   ![Create Virtual Network](screenshots/create-virtual-network.png)

3. **Deploy a Virtual Machine**:
   - Navigate to Virtual Machines and click **+ Create**.
   - Configure the VM with an admin user, network, and size.
   ![Create Virtual Machine](screenshots/create-virtual-machine.png)

4. **Connect to the Virtual Machine**:
   - Use RDP (Windows) or SSH (Linux) to connect to the VM.
   ![VM Running](screenshots/vm-running.png)

### Testing
- Ping the Virtual Machine from your local system.
- Verify the IP address using `ipconfig` or `ifconfig` inside the VM.

### Troubleshooting
- **Connection Issues**: Ensure the Network Security Group allows RDP or SSH traffic.
- **Deployment Failures**: Check subscription quotas and region availability.


Tutorial Steps
1. Prerequisites
An active Microsoft Azure account.
Familiarity with the Azure Portal or Azure CLI.
Azure CLI installed (optional, for scripting).



Create a Resource group
<img width="1006" alt="az1" src="https://github.com/user-attachments/assets/fe750b53-5f1c-4905-8a21-c02523d641fd" />
<img width="1920" alt="az2" src="https://github.com/user-attachments/assets/59e618df-22f6-424f-b096-76c675489fa1" />
<img width="1920" alt="az3" src="https://github.com/user-attachments/assets/812490e5-8447-42c8-a26f-0bcdc24c5a2c" />
NAME YOUR RG AND SELECT YOUR REGION





<img width="1920" alt="az4" src="https://github.com/user-attachments/assets/ca8cbd6f-5bf6-4b00-a299-7df3edf1b31e" />
CLICK CREATE
<img width="1920" alt="az8" src="https://github.com/user-attachments/assets/cf88d4d2-cb47-496b-906d-c57e89eb402c" />
<img width="1920" alt="AZVN1" src="https://github.com/user-attachments/assets/3aa24289-7c57-4467-984b-bce011209384" />
<img width="1920" alt="AZVN2" src="https://github.com/user-attachments/assets/d52fe3eb-d47d-412f-a6b6-b82ce9219c76" />
<img width="964" alt="az7" src="https://github.com/user-attachments/assets/cdc3d8e2-cfe3-4706-97a8-7327b95f4e0c" />


<img width="964" alt="az10" src="https://github.com/user-attachments/assets/b04b7618-46cd-4c76-93ba-af38b960f156" />
<img width="964" alt="az11" src="https://github.com/user-attachments/assets/8d61e7c9-eddb-4ff4-a24a-1b3410300a2c" />
<img width="1920" alt="az12" src="https://github.com/user-attachments/assets/3cfdd1bd-2410-4b03-9d6b-bc60d765344e" />
<img width="1920" alt="az13" src="https://github.com/user-attachments/assets/73bdcf16-2618-4b16-befa-dc28bdd63d66" />
<img width="1920" alt="az14" src="https://github.com/user-attachments/assets/74995cbb-247e-47dc-9d43-4909f12b3cbd" />
<img width="1920" alt="az15" src="https://github.com/user-attachments/assets/837593dc-0cfa-4305-a189-37aad7a001ce" />


