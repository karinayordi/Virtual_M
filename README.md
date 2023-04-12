<p>
<h1>Create a Windows virtual machine in the Azure portal</h1>
<p>
<img src="https://i.imgur.com/OckOSyT.png" height="80%" width="80%" 
</p>
<h1>What is a virtual machine?</h1>
A Virtual Machine (VM) is a compute resource that uses software instead of a physical computer to run programs and deploy apps. One or more virtual “guest” machines run on a physical “host” machine.  Each virtual machine runs its own operating system and functions separately from the other VMs, even when they are all running on the same host. This means that, for example, a virtual MacOS virtual machine can run on a physical PC. 

Virtual machine technology is used for many use cases across on-premises and cloud environments. More recently, public cloud services are using virtual machines to provide virtual application resources to multiple users at once, for even more cost efficient and flexible compute.  
</p>

<h2>Requirements</h2>

* Computer with Internet Connection
* If you don't have an Azure subscription, create a free account before you begin.

<h2>Sign in to Azure</h2>

Sign in to the Azure portal at https://portal.azure.com.

<h2>Create virtual machine</h2>
1. Enter virtual machines in the search.
</p>
2. Under Services, select Virtual machines.
</p>
3. In the Virtual machines page, select Create and then Azure virtual machine. The Create a virtual machine page opens.
</p>
4. Under Instance details, enter myVM for the Virtual machine name and choose Windows Server 2019 Datacenter - Gen 2 for the Image. Leave the other defaults.
  
  <p>
<img src="https://i.imgur.com/7XFaIYK.png" height="80%" width="80%" 
</p>
<img src="https://i.imgur.com/LamTOnJ.png" height="80%" width="80%" 
</p>

5. Under Administrator account, provide a username, such as azureuser and a password. The password must be at least 12 characters long and meet the defined complexity requirements.
</p>

 <p>
<img src="https://i.imgur.com/WWGINmG.png" height="80%" width="80%" 
</p>

6. Under Inbound port rules, choose Allow selected ports and then select RDP (3389) and HTTP (80) from the drop-down.
</p>

<p>
<img src="https://i.imgur.com/08yp4Z0.png" height="80%" width="80%" 
</p>

7. Leave the remaining defaults and then select the Review + create button at the bottom of the page.
</p>

<p>
<img src="https://i.imgur.com/uPslhC4.png" height="80%" width="80%" 
</p>
  
 8. After validation runs, select the Create button at the bottom of the page.
</p>

<p>
<img src="https://i.imgur.com/jJeSyxQ.png" height="80%" width="80%" 
</p>

 9. After deployment is complete, select Go to resource.
</p>

<p>
<img src="https://i.imgur.com/ORsbcEU.png" height="80%" width="80%" 
</p>
  
<h2>Connect to Virtual Machine</h2>
</p>

<p>
Create a remote desktop connection to the virtual machine. These directions tell you how to connect to your VM from a Windows computer. On a Mac, you need an RDP client such as this Remote Desktop Client from the Mac App Store.
</p>

 1. On the overview page for your virtual machine, select the Connect > RDP.
</p>

<p>
<img src="https://i.imgur.com/JrCU2aa.png" height="80%" width="80%" 
</p>

 2. In the Connect with RDP tab, keep the default options to connect by IP address, over port 3389, and click Download RDP file.
</p>

<p>
<img src="https://i.imgur.com/zzIVd7d.png" height="80%" width="80%" 
</p>
  
3. Open the downloaded RDP file and click Connect when prompted.
</p>

4. In the Windows Security window, select More choices and then Use a different account. Type the username as localhost\username, enter the password you created for the virtual machine, and then click OK.
</p>

5. You may receive a certificate warning during the sign-in process. Click Yes or Continue to create the connection.
</p>
