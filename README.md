# Azure Detection Lab using Microsoft Sentinal 📜📊

## Objective
✨ The Microsoft Azure Detection Lab using Sentinel is a dedicated environment designed for cybersecurity professionals to enhance their threat detection and response skills within Azure environments. This practical aims to configure and deploy Azure resources such as Log Analytics Workspace, Virtual Machines, and Azure Sentinel, with custom analytic rules to detect Microsoft Security Events.


### Skills Learned

- Deploying Azure Resources such as Log Analytics Workspace, Virtual Machines, and Azure Sentinel.
- Configuring data connectors to allow data to be brought into sentinal for analysis.
- Understanding of a new Azure language (KQL) to query logs.
- Searching log data and creating custom rules for data analysis.


## Steps

✨ LAB NAME: Azure Detection Lab using Microsoft Sentinal

✨ OBJECTIVE: The aim is to configure and deploy Azure resources using sentinal to extract and observe log data into one centralized location.

✨ THEORY: Connectors will be used as pre-built methods to connect the API calls.




*Ref 1: 
A resource group and a virtual machine were deployed
<img width="1266" alt="azure vm build 1" src="https://github.com/nathanielreich2k/AzureSIEM/assets/155709615/e082cf0d-6926-4ca8-bbfc-fd4f189dcb65">


*Ref 2: 
To prevent unauthorized login, network security groups (NSG) are modified ensuring inbound facing ports are configured. The security feature "just in time" provides necessary time-based restrictions while also ensuring the principle of least privilege. 
<img width="1057" alt="azure nsg 2" src="https://github.com/nathanielreich2k/AzureSIEM/assets/155709615/0bf92b03-bb87-4804-ad8f-24c47d261214">


*Ref 3: 
Next, Sentinal is deployed into our resources along with a new data creation rule to bring in log data from our Windows 10 VM.
<img width="975" alt="azure sentinal 3" src="https://github.com/nathanielreich2k/AzureSIEM/assets/155709615/34174970-d180-4120-b140-48f09794887b">

*Ref 4: 
With the public IP, we can connect to the virtual machine and search in the event viewer. For a large company, multiple user accounts could be accessed and modified in this way.
<img width="999" alt="rdp 4" src="https://github.com/nathanielreich2k/AzureSIEM/assets/155709615/2cb2be4c-2317-4066-aabc-55c9b979715d">

*Ref 5: 
Using the search function we can look for a random ID: 4624. Upon clicking information can be brought up and displays a successful login attempt. 
<img width="842" alt="event view 5" src="https://github.com/nathanielreich2k/AzureSIEM/assets/155709615/19ad9a53-5ff2-47f1-aecf-04b3b942194b">

*Ref 6: 
Going back into the Sentinal logs we can use an exclusive language known as KQL to set a custom analytic rule. As shown below, to make our search easier we can include the time of login, node name, and generation dates. 
<img width="664" alt="query 6+" src="https://github.com/nathanielreich2k/AzureSIEM/assets/155709615/028f2a80-a4d4-4683-8659-98086919501e">
<img width="811" alt="query 6" src="https://github.com/nathanielreich2k/AzureSIEM/assets/155709615/65f21642-fd91-4662-87fa-e995de532565">








































