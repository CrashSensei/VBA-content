---
title: Pages.CalloutRelationshipDeleted Event (Visio)
keywords: vis_sdr.chm11062080
f1_keywords:
- vis_sdr.chm11062080
ms.prod: visio
api_name:
- Visio.Pages.CalloutRelationshipDeleted
ms.assetid: 5e5a3149-9179-8e7c-3728-36e7e2cc3c71
ms.date: 06/08/2017
---


# Pages.CalloutRelationshipDeleted Event (Visio)

Occurs when a callout relationship is deleted from a page.


## Syntax

Private Sub  _expression_ _**CalloutRelationshipDeleted**( **_By Val ShapePair As RelatedShapePairEvent_** )

 _expression_ A variable that represents a **[Pages](pages-object-visio.md)** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _ShapePair_|Required| **[RelatedShapePairEvent](relatedshapepairevent-object-visio.md)**|An object that represents the callout shape-pair relationship.|

## Remarks

The  **RelatedShapePairEvent** object that this event returns contains two shapes: the container and the member, represented by the **[RelatedShapePairEvent.FromShapeID](relatedshapepairevent-fromshapeid-property-visio.md)** and the **[RelatedShapePairEvent.ToShapeID](relatedshapepairevent-toshapeid-property-visio.md)** properties respectively. When Microsoft Visio deletes both shapes in the callout relationship simultaneously, for example when both shapes are deleted from a drawing as part of a selection, the event does not fire.

If you are using Microsoft Visual Basic or Visual Basic for Applications (VBA), the syntax in this topic describes a common, efficient way to handle events.

If you want to create your own  **[Event](event-object-visio.md)** objects, use the **[EventList.Add](eventlist-add-method-visio.md)** or **[EventList.AddAdvise](eventlist-addadvise-method-visio.md)** method. To create an **Event** object that runs an add-on, use the **EventList.Add** method. To create an **Event** object that receives notification, use the **EventList.AddAdvise** method. To find an event code for the event that you want to create, see[Event Codes](http://msdn.microsoft.com/library/de8f5c7a-421d-ebcf-22b6-4310a202ef64%28Office.15%29.aspx).


