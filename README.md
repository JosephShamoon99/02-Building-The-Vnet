# 02-Building-The-Vnet

<h2>Overview</h2>
Here is my documentation how I made the basic layout of my Vnet in Azure.
<br /> 

<h2>Making the Vnet</h2>

First things first, like with all Azure projects I first created a resource group to put everything I made inside of it. I just named the resource group, Car Dealership. 

<img width="1920" height="954" alt="Snapshot#1" src="https://github.com/user-attachments/assets/ef7b61c0-0b08-4d15-89cb-ba35fe44ab88" /> 

I then made my Vnet and placed it inside of the Car Dealership resource group. 

<img width="1920" height="955" alt="Snapshot#2" src="https://github.com/user-attachments/assets/e2a3912c-0ea3-4fa4-999d-fabb057f5b6d" /> 

Under the security settings I went ahead and added an Azure Firewall with default settings. This will be the boundary between my virtual environment and the outside internet. 

<img width="1920" height="953" alt="Snapshot#3" src="https://github.com/user-attachments/assets/9f455724-2543-4d2b-b868-ce0510508a3b" /> 

I left the private IP range at it's defalut setting. 

<img width="1920" height="954" alt="Snapshot#4" src="https://github.com/user-attachments/assets/33c7086b-d8f2-4d3e-b5b3-433ec078c971" /> 

I created the Vnet after I was happy with all the settings and you can see my Vnet under the Virtual Networks tab. 

<img width="1920" height="954" alt="Snapshot#5" src="https://github.com/user-attachments/assets/bfa2665a-6291-45ba-bc35-8ba4e2359d15" /> 

I then created my subnets. I clicked on my Vnet > settings > subnets. As you can see I have a default subnet and a subnet for thr Azure Firewall I made. I'll go ahead and just delete the default subnet and make my 
own subnets. 

<img width="1920" height="956" alt="Snapshot#6" src="https://github.com/user-attachments/assets/d9c4292a-88bc-48c4-a420-d44e9d982e37" /> 

I made my Server Subnet first. I gave it a starting IP of 10.0.2.0. The rest of the subnets will follow this pattern  (10.0.2.0 to 10.0.3.0 and so on). I also enabled "Private Subnet" to keep my 
server subnet from having default outbound access for security reasons. I will enable "Private Subnet" for all the subnets I make. 

<img width="1920" height="953" alt="Snapshot#7" src="https://github.com/user-attachments/assets/c1cea294-97f7-49d4-8d9d-0e506630239d" /> 

Here are all the subnets I made for this Lab. 

<img width="1920" height="957" alt="Snapshot#8" src="https://github.com/user-attachments/assets/4fdb4d29-b217-42c6-afbe-0ed28f124fdd" />









