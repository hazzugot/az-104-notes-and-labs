---
course: AZ-104
title: Lab Environment
type: admin
tags:
  - az104
  - admin
---

# Lab Environment

Temporary QA-issued training tenant. Nothing here is production, and the account is disposed of at the end of the course.

## Sign-in

| | |
| --- | --- |
| **Portal** | `https://portal.azure.com` |
| **Entra admin center** | `https://entra.microsoft.com` |


## Lab conventions

- Default region used throughout the labs: **East US**. You can change it, but change it *consistently* — several labs depend on resources being co-located.
- Resource naming: `az104-*` (e.g. `az104-rg1`, `az104-user1`, `az104-vnet1`).
- Most labs assume the previous lab's resources still exist. Read the "Lab scenario" section before deleting anything.

## Housekeeping

- [x] Delete resource groups at the end of each day to avoid credit burn
- [ ] Check **Cost Management > Cost analysis** if the subscription stops letting you deploy

## Useful starting points

- [AZ-104 skills measured (official study guide)](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-104)
- [Microsoft Learn AZ-104 lab directory](https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/)
- [Azure portal Quickstart Center](https://portal.azure.com/#view/Microsoft_Azure_Resources/QuickstartCenterBlade)
