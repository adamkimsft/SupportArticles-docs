---
title: Re-register Windows client/server in WSUS
description: Provides the steps to re-register a Windows client/server in WSUS.
ms.date: 01/15/2025
manager: dcscontentpm
audience: itpro
ms.topic: troubleshooting
ms.reviewer: kaushika
ms.custom:
- sap:windows servicing,updates and features on demand\windows update configuration,settings and management
- pcy:WinComm Devices Deploy
---
# How to re-register Windows client/server in WSUS

This article provides the steps to re-register a Windows client/server in Windows Server Update Services (WSUS).

_Original KB number:_ &nbsp; 555974

## Summary

This article will help you to re-register a Windows client/server in WSUS.

## Tips

To re-register a Windows client/server in WSUS, review the following instructions:

1. Run `gpupdate /force` command on the Windows client/server that have a registration issue in WSUS.

2. Run `wuauclt /detectnow` command on the Windows client/server that have a registration issue in WSUS.

    > [!TIP]
    > You can use the Event Viewer to review the re-registration.

3. In rare cases, you may need to run `wuauclt.exe /resetauthorization /detectnow` command on the Windows client/server that have a registration issue in WSUS.

## Data collection

If you need assistance from Microsoft support, we recommend you collect the information by following the steps mentioned in [Gather information by using TSS for deployment-related issues](../../windows-client/windows-troubleshooters/gather-information-using-tss-deployment.md).

[!INCLUDE [Community Solutions Content Disclaimer](../../includes/community-solutions-content-disclaimer.md)]
