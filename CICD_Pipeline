**Azure DataBricks CICD Pipeline**

<img src="Images\cicd.png" width=600>
<br>
</br>

> **What is CI/CD?** \
> It is a set of practices used to automate and streamline the process of building, testing, and deploying code changes to different Environments

### Agenda:

1. **Triggering Jobs:** The pipeline triggers whenever updates are made to the main branch of the Git repository.
   
2. **Moving Notebooks:** Upon triggering, the pipeline moves notebook files from the workspace/notebook files directory to the Live folder. The Live folder contains notebooks used for data transformation, which are utilized by the Azure Data Factory (ADF) pipeline for daily triggers.

### Continuous Integration (CI):

- **Development Environment (DEV):** 
  - New pull requests made to the main branch in the DEV environment trigger the pipeline.
  - The pipeline moves notebook files from the notebook folder to the Live folder.

### Continuous Deployment (CD):

- **Production Environment (PROD):**
  - Changes made to the Live folder in the PROD environment trigger the pipeline.
  - The pipeline automatically pulls notebook files from the Live folder into the PROD environment's Live folder.

### Repository Rules:

- **Branch Restriction:**
  - Direct commits to the main branch are restricted. Only pull requests are allowed from other branches.
- **Approval Process:**
  - Pull requests require approval from other approvers before they can be completed.

### Tools Used:

- **Azure DevOps:** Used for managing the CI/CD pipeline and version control.
- **Azure Resource Group:** Provides a logical grouping of Azure resources for easier management and access control.
- **Azure Databricks:** Used for running notebooks and performing data analytics tasks.
- **Visual Studio Code (VSCode):** An integrated development environment (IDE) used for editing code and managing Git repositories.

## Reference:

https://youtu.be/Ievfk8sBTyw?list=PL8zzpRdWG890-ypm8yJJ2zBBvY61MWdER

[Microsoft-hosted agents for Azure Pipelines - Azure Pipelines | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/pipelines/agents/hosted?view=azure-devops&tabs=yaml)

https://learn.microsoft.com/en-us/azure/data-factory/continuous-integration-delivery-improvements

[Azure PowerShell Az module: generate bearer token for Databricks - Stack Overflow](https://stackoverflow.com/questions/62683910/azure-powershell-az-module-generate-bearer-token-for-databricks)


[Invoke-WebRequest (Microsoft.PowerShell.Utility) - PowerShell | Microsoft Learn](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-7.4)

[Configure and pay for parallel jobs - Azure DevOps | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/pipelines/licensing/concurrent-jobs?view=azure-devops&tabs=ms-hosted)

[azure devops - How to resolve "No hosted parallelism has been purchased or granted" in free tier? - Stack Overflow](https://stackoverflow.com/questions/68405027/how-to-resolve-no-hosted-parallelism-has-been-purchased-or-granted-in-free-tie)
