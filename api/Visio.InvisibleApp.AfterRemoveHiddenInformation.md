---
title: InvisibleApp.AfterRemoveHiddenInformation event (Visio)
ms.prod: visio
api_name:
- Visio.InvisibleApp.AfterRemoveHiddenInformation
ms.assetid: 806422e1-66ce-5bed-da8d-5fcdbb2cd662
ms.date: 06/24/2019
ms.localizationpriority: medium
---


# InvisibleApp.AfterRemoveHiddenInformation event (Visio)

Occurs when hidden information is removed from the document.


## Syntax

_expression_.**AfterRemoveHiddenInformation** (_doc_)

_expression_ An expression that returns an **[InvisibleApp](Visio.InvisibleApp.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _doc_|Required| **[IVDOCUMENT]**|The document from which hidden information has been removed.|

## Remarks

The **AfterRemoveHiddenInformation** event is one of a group of events for which the **EventInfo** property of the **Application** object contains extra information.

When the **AfterRemoveHiddenInformation** event is fired, the **EventInfo** property returns a string that contains information about which items were removed from the document, consisting of the sum of applicable constant values from the **[VisRemoveHiddenInfoItems](Visio.visremovehiddeninfoitems.md)** enumeration.

If you are using Microsoft Visual Basic or Visual Basic for Applications (VBA), the syntax in this topic describes a common, efficient way to handle events.

If you want to create your own **Event** objects, use the **[Add](visio.eventlist.add.md)** or **[AddAdvise](visio.eventlist.addadvise.md)** method. 

To create an **Event** object that runs an add-on, use the **Add** method as it applies to the **EventList** collection. 

To create an **Event** object that receives notification, use the **AddAdvise** method. 

To find an event code for the event that you want to create, see [Event codes](../visio/Concepts/event-codesvisio.md).

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]