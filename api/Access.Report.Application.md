---
title: Report.Application property (Access)
keywords: vbaac10.chm13778
f1_keywords:
- vbaac10.chm13778
ms.prod: access
api_name:
- Access.Report.Application
ms.assetid: 2fb2ca56-bbc9-e689-08f3-d42fa97f21d2
ms.date: 03/15/2019
ms.localizationpriority: medium
---


# Report.Application property (Access)

Use the **Application** property to access the active Microsoft Access **[Application](Access.Application.md)** object and its related properties. Read-only **Application** object.


## Syntax

_expression_.**Application**

_expression_ A variable that represents a **[Report](Access.Report.md)** object.


## Remarks

The **Application** property is set by Microsoft Access and is read-only in all views.

Each Microsoft Access object has an **Application** property that returns the current **Application** object. Use this property to access any of the object's properties. For example, you could refer to the menu bar for the **Application** object from the current form by using the following syntax.

```vb
Me.Application.MenuBar 

```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]