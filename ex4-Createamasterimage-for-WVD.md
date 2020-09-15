# Exercise 7: Create a master image for WVD

In this exercise we are going to walk through the process of creating a master image for your WVD host pools. The basic concept for a master image is to start with a clean base install of Windows and layer on mandatory updates, applications and configurations. There are many ways to create and manage images for WVD. The steps covered in this exercise are going to walk you through a basic build and capture process that includes core applications and recommended configuration options for WVD.

## **Task 1: Create a new Virtual Machine in Azure**

1. On the Azure portal home page, Select Create a resource.

![ws name.](media/e1.png)

2. Search and select **Microsoft Windows 10**.

![ws name.](media/e2.png)

3. From dropdown menu select **Windows 10 Enterprise multi-session, Version 1909** and click on create **Create**.

![ws name.](media/e3.png)

4. Provide the below configuration for the virtual machine, and click on **Review + create** and then click on **create**.

![ws name.](media/e4.png)

- Name: wvdwin10
- Region: (default region of resource group)
- Image: **Windows 10 Enterprise multi-session, Version 1909-Gen1**
- size: Standard_D2s_v3
- Username: azuser
- Password: Azure1234567
- Public inbound ports: select **Allow selected ports**
- Select inbound ports: RDP(3389)

