![image](https://github.com/user-attachments/assets/f4a86f09-09b8-4ab5-870b-a2de3c588e6f)


# Virtual Networks and Virtual Machines

 - # Prerequisites:
  
   -Microsoft Account
   
   -Azure account made through the Azure Portal, using your Microsoft credentials
   
   -Connection to Internet


# Creating Our Resource Group

This is the Azure Portal Home Screen. In the search bar search for Resource Groups, the icon looks like this:

![image](https://github.com/user-attachments/assets/8840be5e-2938-42c3-9491-36236b95d048) 
![image](https://github.com/user-attachments/assets/a9410ac6-2f33-4804-8ebf-04cf37d6e9c0)

A resource group in Azure is a container that organizes and manages related resources like virtual machines, storage, and applications

When you go to Resource Groups, in the top left it will say "Create Resource Group" and this page will come up. Use your subscription you used to set up your Azure account, name your group, and then select your region.
![image](https://github.com/user-attachments/assets/67e7fcf4-c811-4240-b804-efcc934b2856) ![image](https://github.com/user-attachments/assets/65d871e4-1ddf-4116-b3ed-ecf4e456d56f)

After you set your subscription, name, and region, click through review and create.
![image](https://github.com/user-attachments/assets/048a1570-e93c-4d8e-8269-5c52739f198c)

# Creating our Virtual Network

Go back to the Azure homepage and search for Virtual Networks, or click the icon at the top toolbar. It will look like this, click create 

![image](https://github.com/user-attachments/assets/76e16e5b-e6fe-4242-947a-cdfe58f0d433)

Next it will bring you here, make sure the Resource Group that the Virtual Network is connected to is the same one you just created. Name your network whatever you want to. Then click through to review and create.
![image](https://github.com/user-attachments/assets/822ad8f3-e7fb-4e37-96b6-382b23813fad) ![image](https://github.com/user-attachments/assets/46df5f17-ec85-47c2-a387-263a177f74ec)

To make sure this is done correctly, go to the Azure homepage, go to resource groups, click the one that was just made, and you should see the virtual network is contained within the resource group.
![image](https://github.com/user-attachments/assets/88720488-9455-4a77-9233-23f2b25ab309)

# Virtual Machine Creation 

Same as before, search for Virtual Machines in the Azure search bar, or click it on the toolbar.

![image](https://github.com/user-attachments/assets/e0f8af77-ce82-426c-a9cd-193f9bd6bbad)

Click Create Azure Virtual Machine and ensure you have the correct resource group selected. Name your VM whatever you want.
![image](https://github.com/user-attachments/assets/05090dd1-f007-4f68-aa64-375e488ac63a) 
![image](https://github.com/user-attachments/assets/4e0f5316-9505-44ad-bc57-235e6c767782)

Next select your image, this is the OS the machine will be running. All other settings shown in picture don't get changed. For this demonstration, I will be using this OS and size:
![image](https://github.com/user-attachments/assets/888e243e-e86a-4f5d-b05c-fc570930acad)


For the demo, I will be using account name user123 and the password is Password1234. This isn't smart to do for real use but okay for a demo.
![image](https://github.com/user-attachments/assets/6e1c0e50-1438-47df-9881-f059a0c1ac32)

Be sure to check the box at the bottom of the page as it will not work if you don't check it!

![image](https://github.com/user-attachments/assets/0ca31c04-8e9d-41b8-9726-7c12e3aef6ff)

Click next which will bring you to Disks. Click next again and it will bring you to Networking. Set the Virtual Network to same one we created earlier. 
![image](https://github.com/user-attachments/assets/77217b1f-8026-4935-9d8c-2f956b326f2f)


Click through to Review and Create and wait for the deployment to finish. Once deployment is finished go to resource groups and click on the one that we created for our network and machines. If done successfully, it will look like this, with everything needed for our virtual network an virtual machine contained in the same resource group:

![image](https://github.com/user-attachments/assets/bd6c97db-4119-4d15-b26a-9937ad087d95)

This demonstration is now complete. This showed how to configure a Virtual Network and Virtual Machines in Azure. We are able to add more machines to the network by following the same steps used above, and both VMs would be on the same Virtual Network! 
