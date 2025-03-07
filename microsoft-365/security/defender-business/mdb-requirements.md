---
title: Requirements for Microsoft Defender for Business
description: Microsoft Defender for Business license, hardware, and software requirements
search.appverid: MET150
author: denisebmsft
ms.author: deniseb
manager: dansimp 
audience: Admin
ms.topic: overview
ms.service: microsoft-365-security
ms.subservice: mdb
ms.localizationpriority: medium
ms.date: 01/26/2023
ms.reviewer: shlomiakirav
f1.keywords: NOCSH 
ms.collection: 
 - SMB
 - m365-security
 - m365solution-mdb-setup
 - highpri
 - tier1
---

# Microsoft Defender for Business requirements

This article describes the requirements for Defender for Business.

## What to do

1. [Review the requirements and make sure you meet them](#review-the-requirements).
2. [Proceed to your next steps](#next-steps).


## Review the requirements

The following table lists the basic requirements you need to configure and use Defender for Business.

| Requirement | Description |
|:---|:---|
| Subscription | Microsoft 365 Business Premium or Defender for Business (standalone). See [How to get Defender for Business](get-defender-business.md).  |
| Datacenter | One of the following datacenter locations: <ul><li>European Union</li><li>United Kingdom</li><li>United States</li></ul> |
| User accounts |<ul><li>User accounts are created in the Microsoft 365 admin center ([https://admin.microsoft.com](https://admin.microsoft.com)).</li><li>Licenses for Defender for Business (or Microsoft 365 Business Premium) are assigned in the Microsoft 365 admin center.</li></ul>To get help with this task, see [Add users and assign licenses](mdb-add-users.md). |
| Permissions  | To sign up for Defender for Business, you must be a Global Admin.<br/><br/>To access the Microsoft 365 Defender portal, users must have one of the following [roles in Azure AD](mdb-roles-permissions.md) assigned:<ul><li>Security Reader</li><li>Security Admin</li><li>Global Admin</li></ul>To learn more, see [Roles and permissions in Defender for Business](mdb-roles-permissions.md). |
| Browser requirements | Microsoft Edge or Google Chrome |
| Client device operating system | To manage devices in the Microsoft 365 Defender portal, your devices must be running one of the following operating systems: <ul><li>Windows 10 or 11 Business</li><li>Windows 10 or 11 Professional</li><li>Windows 10 or 11 Enterprise</li><li>Mac (the three most-current releases are supported)</li></ul>Make sure that [KB5006738](https://support.microsoft.com/topic/october-26-2021-kb5006738-os-builds-19041-1320-19042-1320-and-19043-1320-preview-ccbce6bf-ae00-4e66-9789-ce8e7ea35541) is installed on the Windows devices. <br/><br/>If you're already managing devices in Microsoft Intune, you can continue to use it.<sup>[[1](#fn1)]</sup> In that case, the following other operating systems are supported: <ul><li>iOS and iPadOS</li><li>Android OS</li></ul> |
| Server requirements | To onboard a device running Windows Server or Linux Server, you'll need an additional license, such as [Microsoft Defender for Business servers](get-defender-business-servers.md)<sup>[[2](#fn2)]</sup>.<br/><br/>Windows Server endpoints must meet the [requirements for Defender for Endpoint](/microsoft-365/security/defender-endpoint/minimum-requirements#hardware-and-software-requirements), and enforcement scope must be turned on.<ol><li>In the Microsoft 365 Defender portal, go to **Settings** > **Endpoints** > **Configuration management** > **Enforcement scope**.</li><li>Select **Use MDE to enforce security configuration settings from MEM**, select  **Windows Server**. </li><li>Select **Save**.</li></ol>Linux Server endpoints must meet the [prerequisites for Microsoft Defender for Endpoint on Linux](../defender-endpoint/microsoft-defender-endpoint-linux.md#prerequisites).|

(<a id="fn1">1</a>) Microsoft Intune is not included in the standalone version of Defender for Business. Intune can be added onto Defender for Business. Intune is included in Microsoft 365 Business Premium.

(<a id="fn2">2</a>) To onboard servers, we recommend using [Microsoft Defender for Business servers](get-defender-business-servers.md). Alternately, you could use [Microsoft Defender for Servers Plan 1 or Plan 2](/azure/defender-for-cloud/plan-defender-for-servers). To learn more, see [What happens if I have a mix of Microsoft endpoint security subscriptions?](mdb-faq.yml#what-happens-if-i-have-a-mix-of-microsoft-endpoint-security-subscriptions) and [Onboard devices to Microsoft Defender for Business](mdb-onboard-devices.md).

> [!NOTE]
> [Azure Active Directory (Azure AD)](/azure/active-directory/fundamentals/active-directory-whatis) is used to manage user permissions and device groups. Azure AD is included in your Defender for Business subscription. 
> - If you don't have a Microsoft 365 subscription before you start your trial, Azure AD will be provisioned for you during the activation process. 
> - If you do have another Microsoft 365 subscription when you start your Defender for Business trial, you can use your existing Azure AD service. 

## Next steps

- If you don't already have Defender for Business, see [Get and provision Microsoft Defender for Business](get-defender-business.md).
- If you're starting a trial subscription, see the [Trial user guide: Microsoft Defender for Business](trial-playbook-defender-business.md).
- If you're ready to set up Defender for Business for your organization, see [Set up and configure Microsoft Defender for Business](mdb-setup-configuration.md).
