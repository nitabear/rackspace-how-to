---
permalink: adding-disk-space-after-resizing-a-windows-2003-cloud-server/
node_id: 1296
title: Add Disk Space After Resizing a Windows 2003 Cloud Server
type: article
created_date: '2012-03-01'
created_by: Rackspace Support
last_modified_date: '2016-01-21'
last_modified_by: Zach Corleissen
product: Cloud Servers
product_url: cloud-servers
---

**Note**:  Rackspace no longer offers Cloud Servers with Windows 2003, but these instructions are here for legacy support purposes.

### Formatting the Disk and Adding an Additional Drive

-   Log into your Windows Server 2003 Cloud Server using Remote Desktop
    and logging in as the user Administrator, or with an account that is
    part of the Administrator group.

  <img src="{% asset_path cloud-servers/adding-disk-space-after-resizing-a-windows-2003-cloud-server/RDPConnectExample.png %}" alt="" />

-   From the Desktop of your Windows Server 2003 Cloud Server, open
    the **Start Menu** and select **Administrative
    Tools > Computer Management**.

  <img src="{% asset_path cloud-servers/adding-disk-space-after-resizing-a-windows-2003-cloud-server/Win2003AdminTools.png %}" alt="" />

-   Under the **Storage** folder in the left pane, select **Disk
    Management**.  In the left pane of Disk Management you will see the
    current formatted hard drive for your server, and you should also
    see an amount of unallocated space in the right pane.  Right-click
    on the Unallocated space and choose **New Partition** from the menu.

  <img src="{% asset_path cloud-servers/adding-disk-space-after-resizing-a-windows-2003-cloud-server/Win2003NewPartition.png %}" alt="" />

-   This will open the **New Partition Wizard** screen.
     Press **Next** to begin.

  <img src="{% asset_path cloud-servers/adding-disk-space-after-resizing-a-windows-2003-cloud-server/Win2003NewPartitionWizard.png %}" alt="" />

-   **Select Partition Type** - Check the radio button next
    to **Primary partition **and click **Next. **

  <img src="{% asset_path cloud-servers/adding-disk-space-after-resizing-a-windows-2003-cloud-server/Win2003PrimaryPartition.png %}" alt="" />

-   **Specify Partition Size** - Next you will be asked to specify the
    partition size.  If you want to add all of your available disk space
    to one new partition, go ahead and accept the default settings and
    press **Next**.  If you only want to use a portion of your available
    disk space for the new partition, you can specify the amount of
    space to use in the **Partition size in MB** field.

  <img src="{% asset_path cloud-servers/adding-disk-space-after-resizing-a-windows-2003-cloud-server/Win2003SpecifyPartitionSize.png %}" alt="" />

-   **Assign Drive Letter** - Choose the drive letter for your new
    volume and click **Next**.

  <img src="{% asset_path cloud-servers/adding-disk-space-after-resizing-a-windows-2003-cloud-server/Win2003AssignDriveLetter.png %}" alt="" />

-   **Format Partition** - Format the partition as an NTFS partition.
     Here you can also name the partition, such as "New Volume" in
    this example.  Keep the default settings on this screen, and
    press **Next**.

  <img src="{% asset_path cloud-servers/adding-disk-space-after-resizing-a-windows-2003-cloud-server/Win2003FormatPartition.png %}" alt="" />

-   **Complete the New Partition Wizard** - You have now successfully
    created and formatted a new partition as the destination for the
    newly available hard drive space that has been added to your Windows
    Server 2003 Cloud Server.  Press the **Finish** button to complete
    the process.

  <img src="{% asset_path cloud-servers/adding-disk-space-after-resizing-a-windows-2003-cloud-server/Win2003CompleteNewPartWiz3.png %}" alt="" />

-   You will now see the additional disk drive volume that you created.
     Close Computer Management and begin using the additional space that
    you have just created.

  <img src="{% asset_path cloud-servers/adding-disk-space-after-resizing-a-windows-2003-cloud-server/Win2003driveCandD.png %}" alt="" />
