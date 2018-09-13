# Black Duck CoPilot Gradle/Travis CI Example



Shows a working setup for using the Black Duck CoPilot integration to analyze the risk of project dependencies

## Azure Pipelines Setup

The `azure-pipelines.yml` file has been modified to upload generated dependency data to Black Duck CoPilot:

```yaml
- script: bash <(curl -s https://copilot-valid.blackducksoftware.com/ci/azure/scripts/upload)
```

