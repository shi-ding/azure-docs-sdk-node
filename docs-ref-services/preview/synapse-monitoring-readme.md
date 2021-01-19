---
title: Azure Synapse Monitoring client library for JavaScript
keywords: Azure, javascript, SDK, API, @azure/synapse-monitoring, 
author: maggiepint
ms.author: magpint
ms.date: 12/09/2020
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: javascript
ms.service: 
---

## Azure Synapse Monitoring client library for JavaScript - Version 1.0.0-beta.1 


This package contains an isomorphic SDK for Monitoring.

## Getting started

### Install the package

```bash
npm install @azure/synapse-monitoring
```

### Currently supported environments

- Node.js version 8.x.x or higher
- Browser JavaScript

## Key concepts

## Examples

```ts
import { MonitoringClient } from "@azure/synapse-monitoring";
import { DefaultAzureCredential } from "@azure/identity";

export async function main(): Promise<void> {
  const credential = new DefaultAzureCredential();

  let client = new MonitoringClient(credential, "https://mysynapse.dev.azuresynapse.net");
  let output = await client.monitoring.getSparkJobList();
  console.log("output:", output);
}
```

## Related projects

- [Microsoft Azure SDK for Javascript](https://github.com/Azure/azure-sdk-for-js)

![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-js%2Fsdk%2Fcdn%2Farm-cdn%2FREADME.png)

## Troubleshooting

Enabling logging may help uncover useful information about failures. In order to see a log of HTTP requests and responses, set the `AZURE_LOG_LEVEL` environment variable to `info`. Alternatively, logging can be enabled at runtime by calling `setLogLevel` in the `@azure/logger`:

```javascript
import { setLogLevel } from "@azure/logger";

setLogLevel("info");
```

## Next steps

In the future, you'll find additional code samples here.

## Contributing

If you'd like to contribute to this library, please read the [contributing guide](https://github.com/Azure/azure-sdk-for-js/blob/@azure/synapse-monitoring_1.0.0-beta.1/CONTRIBUTING.md) to learn more about how to build and test the code.

![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-js%2Fsdk%2Fkeyvault%2Fkeyvault-keys%2FREADME.png)
