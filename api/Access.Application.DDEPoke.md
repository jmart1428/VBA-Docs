---
title: Application.DDEPoke method (Access)
keywords: vbaac10.chm12541
f1_keywords:
- vbaac10.chm12541
ms.prod: access
api_name:
- Access.Application.DDEPoke
ms.assetid: 5f24d625-bd9b-41fd-004c-dccfb0ec41b6
ms.date: 02/05/2019
ms.localizationpriority: medium
---


# Application.DDEPoke method (Access)

Use the **DDEPoke** statement to supply text data from a client application to a server application over an open dynamic data exchange (DDE) channel.


## Syntax

_expression_.**DDEPoke** (_ChanNum_, _Item_, _Data_)

_expression_ A variable that represents an **[Application](Access.Application.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _ChanNum_|Required|**Variant**| A channel number, an integer returned by the **[DDEInitiate](Access.Application.DDEInitiate.md)** function.|
| _Item_|Required|**String**|The name of a data item recognized by the application specified by the **DDEInitiate** function. Check the application's documentation for a list of possible items.|
| _Data_|Required|**String**|The data to be supplied to the other application.|

## Remarks

For example, if you have an open DDE channel between Microsoft Access and Microsoft Excel, you can use the **DDEPoke** statement to transfer text from an Access database to an Excel spreadsheet. In this example, Access acts as the client application, and Excel acts as the server application.

The value of the _item_ argument depends on the application and topic specified when the channel indicated by the _channum_ argument is opened. For example, the _item_ argument may be a range of cells in an Excel spreadsheet.

The string contained in the _data_ argument must be an alphanumeric text string. No other formats are supported. For example, the _data_ argument could be a number to fill a cell in a specified range in an Excel worksheet.

If the _channum_ argument isn't an integer corresponding to an open channel, or if the other application doesn't recognize or accept the specified data, a run-time error occurs.

If you need to manipulate another application's objects from Access, you may want to consider using Automation.




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]