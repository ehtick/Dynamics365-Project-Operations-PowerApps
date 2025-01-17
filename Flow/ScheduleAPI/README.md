---
page_type: sample
languages:
- logicflow
products:
- dynamics-project-operations
description: "Dynamics 365 Project Operations Schedule API Flow Sample"
---

# Dynamics 365 Project Operations Schedule API Flow Sample
This a repository to showcase how to use the ScheduleAPIs from flow.   

# Documetation

1. Power Automate: https://learn.microsoft.com/en-us/power-automate/getting-started
2. Schedule API with Power Automate: https://learn.microsoft.com/en-us/dynamics365/project-operations/project-management/scheduling-apis-powerautomate

# Usage

1. Download the solution zip file
2. Go to https://make.powerapps.com/. Select the environment you want to use
3. Import the solution zip file, using the 'Import canvas app' option
4. You will have to update the Data Verse connections
5. After import, navigate to Flows > Cloud flows. You should see a 'PROJOPS DEMO FLOW'
![image](https://user-images.githubusercontent.com/15526549/198174265-a9ac486d-b079-47e7-9181-3554429d472c.png)

This sample shows how to use ScheduleAPI to create Project, ProjectTeamMember, Project Tasks and Assignments.
This flow does the following:
 - creates a Project using msdyn_CreateProjectV1 action
 - creates a Project TeamMember using msdyn_CreateTeamMemberV1 action
 - creates a ProjectBucket using the oData endpoint
 - creates an OperationSet using the msdyn_CreateOperationSetV1 action
 - uses msdyn_PssCreateV1 action to add requests to create 5 Tasks and 5 Assignments to the operationset
 - calls msdyn_ExecuteOperationSetV1 action to execute the operationSet

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
