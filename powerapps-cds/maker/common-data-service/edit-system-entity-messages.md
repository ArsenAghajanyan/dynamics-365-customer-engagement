---
title: "Edit system entity messages with PowerApps | MicrosoftDocs"
description: "Learn how to edit system entity messages"
ms.custom: ""
ms.date: 05/15/2018
ms.reviewer: ""
ms.service: "crm-online"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
applies_to: 
  - "Dynamics 365 (online)"
  - "Dynamics 365 Version 9.x"
  - "powerapps"
author: "Mattp123"
ms.assetid: 3ccbd8de-8d6f-4058-87f7-15463667cfc6
caps.latest.revision: 41
ms.author: "matp"
manager: "kvivek"
---
# Edit system entity messages

The default display name of some system entities is used in user interface text and error messages in Common Data Service for Apps. If you change the display name, you should also update any messages that use the default display name. For example, if you change the display name from *Account* to *Company*, you could still see an error message using the old name.  

You cannot edit system messages using the PowerApps portal you must use solution explorer.

[!INCLUDE [cc_navigate-solution-from-powerapps-portal](../../includes/cc_navigate-solution-from-powerapps-portal.md)]

In the solution explorer, below the entity, if you see a **Messages** node you can edit certain text that includes references to the original entity display name. Editing this text is straightforward. Open the message to see a form with three fields:  
  
|Field|Description|  
|-----------|-----------------|  
|**Default Display String**|Shows the original text.|  
|**Custom Display String**|Edit this text to change the display string.|  
|**Comment**|Optional. Include a comment about what you changed and why.|  
  
 Some of the message text may have placeholders in them. These placeholders are numbers with brackets on either side. For example: `{0}`. These placeholders allow for text to be inserted  in the message. If you edit messages, make sure that you keep these placeholders. 
 
### See also
[Edit an entity](edit-entities.md)