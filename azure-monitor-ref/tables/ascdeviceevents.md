---
title: Azure Monitor Logs reference - ASCDeviceEvents
description: Reference for ASCDeviceEvents table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 2/23/2023
---

# ASCDeviceEvents

 Contains event details for operations generated by Azure Sphere devices. These logs contain information about event types, event categories, event classes, event descriptions etc. that can be used for monitoring and troubleshooting app crashes on devices.

## Categories

- Azure Resources
- Audit
## Solutions

- LogManagement
## Resource types

- Azure Sphere




## Columns

| Column | Type | Description |
| --- | --- | --- |
| CatalogId | string | The catalog ID of the device where the log event was generated. |
| CorrelationId | string | A unique correlation ID for the log event. |
| DeviceId | string | The ID of the device where the log event was generated. |
| DurationMs | int | The total duration (in milliseconds) for the log event. |
| Location | string | The location and region where the log event was generated. |
| OperationName | string | The Azure Sphere operation associated with the log event. |
| Properties | dynamic | Additional properties related to the log event. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| ResultDescription | string | The result description for the log event. |
| ResultType | string | The result type (success, failure) for the log event. |
| SourceSystem | string |  |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string |  |
| TimeGenerated | datetime | Timestamp(UTC) when the log event was generated. |
| Type | string | The name of the table |
