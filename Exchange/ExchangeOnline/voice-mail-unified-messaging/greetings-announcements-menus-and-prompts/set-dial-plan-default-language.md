---
localization_priority: Normal
description: You can set the default language for a Unified Messaging (UM) dial plan. Each dial plan you create will initially use English (en-US) as the default language.
ms.topic: article
author: chrisda
ms.author: chrisda
ms.assetid: 7a1d2e7e-4053-40af-9ec1-ec714df12ad4
ms.date: 7/12/2018
ms.reviewer: 
title: Set the default language on a dial plan
ms.collection: exchange-online
audience: ITPro
ms.service: exchange-online
manager: dansimp

---

# Set the default language on a dial plan

### Use the EAC to set the default language on a UM dial plan

1. In the EAC, navigate to **Unified Messaging** \> **UM dial plans**.

2. In the list view, select the UM dial plan that you want to modify, and then, on the toolbar, click **Edit** ![Edit icon](../../media/ITPro_EAC_EditIcon.gif).

3. On the **UM dial plan** page, click **Configure**.

4. On the **Settings** page, under **Audio language**, select the language you want to set from the drop-down list.

5. Click **Save** to accept your changes.

### Use Exchange Online PowerShell to set the default language on a UM dial plan

This example sets the default language on a UM dial plan named `MyUMDialPlan` to German.

```
Set-UMDialPlan -Identity MyUMDialPlan -DefaultLanguage de-DE
```

This example sets the default language on a UM dial plan named `MyUMDialPlan` to Japanese.

```
Set-UMDialPlan -Identity MyUMDialPlan -DefaultLanguage ja-JP
```

This example sets the default language on a UM dial plan named `MyUMDialPlan` to Australian English.

```
Set-UMDialPlan -Identity MyUMDialPlan -DefaultLanguage en-AU
```



