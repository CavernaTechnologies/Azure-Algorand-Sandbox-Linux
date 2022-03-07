# Deploying Sandbox to a Linux VM in Azure

This repository is here to serve as a resource for deploying an Algorand Sandbox in the cloud. If you'd like to see a step by step guide on how to do this you can see the [Tutorial](https://github.com/CavernaTechnologies/Azure-Algorand-Sandbox-Linux/blob/main/Tutorial.md) file. 

If you set up your environment manually and you'd like to check your configuration, you can jump to the next section.

If you'd like instructions on using the Azure template to get a *perfect* environment set up in just minutes, you can just to the section at the bottom. Using a template still requires some set up on the virtual machine itself, but the overall set up time is decreased significantly.

# Comparing Templates

## Accessing your resource group template

To access your resource group template, you'll need to visit the resource group page and access the **Export template** tab as shown in **Figure 1-1**.

![sandboxResourceGroup](https://github.com/CavernaTechnologies/Azure-Algorand-Sandbox-Linux/blob/main/images/sandboxResourceGroupOverview.png?raw=true)

**Figure 1-1**: Resource group and export template

You can then download the template, demonstrated in **Figure 1-2**, or just view it in browser. This template is a JSON file that fully encompasses the set up of your environment and we can use it to compare your set up to my own.

![downloadTemplate](https://github.com/CavernaTechnologies/Azure-Algorand-Sandbox-Linux/blob/main/images/template.png?raw=true)

**Figure 1-2**: Download template

You can now navigate to the [template of my own set up](https://github.com/CavernaTechnologies/Azure-Algorand-Sandbox-Linux/blob/main/Template-Sandbox-Tutorial/template.json) and compare. The templates won't be identical. Certain resources, resource names, and property values may be different. For example, the public IP won't be the same. However, the general structure of your template and the one shown should be very similar.

# Deploying the virtual environment using an Azure Template

If you'd like to deploy the environment using my [included template](https://github.com/CavernaTechnologies/Azure-Algorand-Sandbox-Linux/blob/main/sandbox-environment-template.json), then you can get up and running in just a few minutes! Simply download the template and access the **Deploy a custom template** section in the Azure portal, as shown in **Figure 2-1**.

![deployCustomTemplate](https://github.com/CavernaTechnologies/Azure-Algorand-Sandbox-Linux/blob/main/images/deployCustomTemplate.png?raw=true)

**Figure 2-1**: Deploy a custom template

From here, you will want to choose to **Build your own template in the editor** as illustrated in **Figure 2-2**.

![customDeployment](https://github.com/CavernaTechnologies/Azure-Algorand-Sandbox-Linux/blob/main/images/customDeployment.png?raw=true)

**Figure 2-2**: Build your own template in the editor

Next, you can upload the provided template using the **Load file** button. After the file is loaded, you can click **Save** in the bottom left. Both of these are shown in **Figure 2-3**

![loadFile](https://github.com/CavernaTechnologies/Azure-Algorand-Sandbox-Linux/blob/main/images/loadFile.png?raw=true)

**Figure 2-3**: Load file

Once you load the file, you can create a **Resource Group**, edit the parameters to your needs, add your **SSH Public Key**, and finally click **Review and Create** as shown in **Figure 2-4**.

![parameters](https://github.com/CavernaTechnologies/Azure-Algorand-Sandbox-Linux/blob/main/images/parameters.png?raw=true)

**Figure 2-4**: Parameters

After that has finished validating, you can click **Create** like in **Figure 2-5**.

![create](https://github.com/CavernaTechnologies/Azure-Algorand-Sandbox-Linux/blob/main/images/create.png?raw=true)

Once the resources have finished deployed, you can follow the [Tutorial](https://github.com/CavernaTechnologies/Azure-Algorand-Sandbox-Linux/blob/main/Tutorial.md). Starting from the **Connecting to virtual machine** step! After completing the remainder of the tutorial, you will be all set up!