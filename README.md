# Black Duck CoPilot Gradle/Azure Pipelines Example

[![Build Status](https://dev.azure.com/copilot0022/copilot/_apis/build/status/BlackDuckCoPilot.example-gradle-azure)](https://dev.azure.com/copilot0022/copilot/_build/latest?definitionId=2) [![Black Duck Security Risk](https://copilot-valid.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-gradle-azure/branches/refs%2Fheads%2Fmaster/badge-risk.svg)](https://copilot-valid.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-gradle-azure/branches/refs%2Fheads%2Fmaster)

Shows a working setup for using the Black Duck CoPilot integration to analyze the risk of project dependencies

## Azure Pipelines Setup

The `azure-pipelines.yml` file has been modified to upload generated dependency data to Black Duck CoPilot:

```yaml
- script: bash <(curl -s https://copilot-valid.blackducksoftware.com/ci/azure/scripts/upload)
```

