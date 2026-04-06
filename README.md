# 02-Building-The-Vnet

<h2>Overview</h2>
Here is my documentation how I made the basic layout of my Vnet in Azure.
<br /> 

<h2>Making the Vnet</h2>

First things first, like with all Azure projects I first created a resource group to put everything I made inside of it. I just named the resource group, Car Dealership. 

<img width="768" height="324" alt="Snapshot#1" src="https://github.com/user-attachments/assets/e5f84cde-8a4a-460c-952f-7e95b2eb3f6b" /> 



I then made my Vnet and placed it inside of the Car Dealership resource group. 

<img width="798" height="643" alt="Snapshot#2" src="https://github.com/user-attachments/assets/af5d1f66-652b-4c23-9f0e-2ed04db689b5" />



Under the security settings I went ahead and added an Azure Firewall with default settings. This will be the boundary between my virtual environment and the outside internet. 

<img width="792" height="753" alt="Snapshot#3" src="https://github.com/user-attachments/assets/d1d3ed9a-4a1d-43fd-aed4-975025cd2547" />



I left the private IP range at it's defalut setting. 

<img width="819" height="688" alt="Snapshot#4" src="https://github.com/user-attachments/assets/beb081d7-b3e9-4366-a6d8-837815beae5b" />



I created the Vnet after I was happy with all the settings and you can see my Vnet under the Virtual Networks tab. 

<img width="870" height="267" alt="Snapshot#5" src="https://github.com/user-attachments/assets/3dab308b-26c7-4fa1-a778-d0111d4e9f50" />



I then created my subnets. I clicked on my Vnet > settings > subnets. As you can see I have a default subnet and a subnet for thr Azure Firewall I made. I'll go ahead and just delete the default subnet and make my 
own subnets. 

<img width="1074" height="377" alt="Snapshot#6" src="https://github.com/user-attachments/assets/5665c2b3-056a-485b-bdf2-bbcafa9dfb94" />



I made my Server Subnet first. I gave it a starting IP of 10.0.2.0. The rest of the subnets will follow this pattern  (10.0.2.0 to 10.0.3.0 and so on). I also enabled "Private Subnet" to keep my 
server subnet from having default outbound access for security reasons. I will enable "Private Subnet" for all the subnets I make. 

<img width="847" height="953" alt="Snapshot#7" src="https://github.com/user-attachments/assets/688b56b1-f59f-41f3-bf2d-1be2f86904a9" />


Here are all the subnets I made for this Lab. 

<img width="1072" height="468" alt="Snapshot#8" src="https://github.com/user-attachments/assets/cf277c48-3595-4d86-92f9-1f2c2e853130" />










