## Objective
In this module, we will create our first resource group and examine some of its properties along with viewing what _type_ of resources we're allowed to add. We'll discuss some basic compliance around resource groups and determining where the metadata is stored.  We will also add a basic resource to the group to view how the resources are listed, managed, etc.  Finally, we will complete this module by deleting the resource group along with all of its resources.

## Create a Resource Group
As stated previously, in order to create resources in Azure, we must assign them to a resource group. So let's get started by creating our first resource group.

  1. If you are not there already, go ahead and click on the **Resource Groups** <img src="https://raw.githubusercontent.com/AzureWorkshops/images/master/icons_resource_groups.jpg" style="display: inline; margin:0px 5px;box-shadow: 2px 2px 2px #999;border:1px solid #ccc;"/> in the Azure Portal to open the Resource Groups blade.

  2. At the top of the Resource Groups blade, click on **Add** <img src="https://raw.githubusercontent.com/AzureWorkshops/images/master/icons_add.jpg" style="display: inline; margin:0px 5px;box-shadow: 2px 2px 2px #999;border:1px solid #ccc;"/>. This will open a panel that asks for some basic configuration settings.

  3. Complete the configuration settings with the following:

      * Resource group name: **azworkshops_vnets_demo**
      * Subscription: **_&lt;choose your subscription&gt;_**
      * Resource group location: **_&lt;choose your location&gt;_**

  4. _&lt;Optional&gt;_ Check _Pin to dashboard_ at the bottom of the panel.

  5. Click **Create**.

  6. It should only take a second for the resource group to be created.  Once you click create, the configuration panel closes and returns you to the list of available resource groups.  Your recently created group may not be visible in the list.  Clicking on **Refresh** <img src="https://raw.githubusercontent.com/AzureWorkshops/images/master/icons_add.jpg" style="display: inline; margin:0px 5px;box-shadow: 2px 2px 2px #999;border:1px solid #ccc;"/> at the top of the Resource Groups blade should display your new resource group.

**NOTE:** When you create a resource group, you are prompted to choose a location. Additionally, as you create individual resources, you will also be prompted to choose locations. The location of resource groups and their resources can be different.  This is because resource groups store _metadata_ describing their contained resources; and, due to some type of compliance that your company may adhere to, you may need to store that metadata in a different location than the resources themselves.  For example, if you are a US-based company, you may choose to keep the metadata state-side while creating resources in foreign regions to reduce latency.