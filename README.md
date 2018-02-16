# azure-sharepoint-dev-vm
Azure ARM template for SharePoint 2016 DEV environment

This ARM template uses the following resources:
- 3 Virtual Machines built on Windows Server 2016 Image: One for AD, one for SQL & one for SharePoint
- Each of 3 VMs has public IP and subnet.
- 2017 SQL Sever Image
- 2016 SharePoint Server Image
- Network Security Group enables RDP(for remote connections) & TCP on port 80
- Uses Desired State Configuration to configure AD, SQL & SharePoint
- Creates default web application and one site

Note: Instead of using SharePoint 2016 Azure image, we can install SharePoint on blank Windows Server 2016