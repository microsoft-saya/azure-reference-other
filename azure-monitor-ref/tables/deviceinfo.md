---
title: Azure Monitor Logs reference - DeviceInfo
description: Reference for DeviceInfo table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: robb
author: rboucher
ms.date: 2/23/2023
---

# DeviceInfo

 This table is part of Microsoft Defender for Endpoints with Azure Sentinel. This table contains Machine information, including OS information.

## Categories

- Security
## Solutions

- Microsoft Sentinel




## Columns

| Column | Type | Description |
| --- | --- | --- |
| AadDeviceId | string | Unique identifier for the device in Azure Active Directory. |
| AdditionalFields | dynamic | Additional information about the entity or event. |
| ClientVersion | string | Version of the endpoint agent or sensor running on the machine. |
| DeviceCategory | string | Broader classification that groups certain device types under the following categories: Endpoint, Network device, IoT, Unknown. |
| DeviceId | string | Unique identifier for the device in the service. |
| DeviceName | string | Fully qualified domain name (FQDN) of the device. |
| DeviceObjectId | string | Unique identifier for the device in Azure AD. |
| DeviceSubtype | string | Additional modifier for certain types of devices, for example, a mobile device can be a tablet or a smartphone; only available if device discovery finds enough information about this attribute. |
| DeviceType | string | Type of device based on purpose and functionality, such as network device, workstation, server, mobile, gaming console, or printer. |
| IsAzureADJoined | bool | Boolean indicator of whether machine is joined to the Azure Active Directory. |
| JoinType | string | The device's Azure Active Directory join type. |
| LoggedOnUsers | dynamic | List of all users that are logged on the machine at the time of the event in JSON array format. |
| MachineGroup | string | Machine group used to determine access to the machine and apply group-specific settings. |
| MergedDeviceIds | string | Previous device IDs that have been assigned to the same device. |
| MergedToDeviceId | string | The most recent device ID assigned to a device. |
| Model | string | Model name or number of the product from the vendor or manufacturer, only available if device discovery finds enough information about this attribute. |
| OnboardingStatus | string | Indicates whether the device is currently onboarded or not to Microsoft Defender for Endpoint or if the device is not supported. |
| OSArchitecture | string | Architecture of the operating system running on the machine. |
| OSBuild | long | Build version of the operating system running on the machine. |
| OSDistribution | string | Distribution of the OS platform, such as Ubuntu or RedHat for Linux platforms. |
| OSPlatform | string | Platform of the operating system running on the machine. This indicates specific operating systems, including variations within the same family, such as Windows 10 and Windows 7. |
| OSVersion | string | Version of the operating system running on the machine. |
| OSVersionInfo | string | Additional information about the OS version, such as the popular name, code name, or version number. |
| PublicIP | string | Public IP address used by the onboarded machine to connect to the Windows Defender ATP service. This could be the IP address of the machine itself, a NAT device, or a proxy. |
| RegistryDeviceTag | string | Device tag added through the registry. |
| ReportId | long | Event identifier based on a repeating counter. To identify unique events, this column must be used in conjunction with the ComputerName and EventTime columns.. |
| SourceSystem | string |  |
| TenantId | string |  |
| TimeGenerated | datetime | Date and time the event was recorded by the MDE agent on the endpoint. |
| Type | string | The name of the table |
| Vendor | string | Name of the product vendor or manufacturer, only available if device discovery finds enough information about this attribute. |
