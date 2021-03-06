---
title: ReferencesEvents property (VBA Add-In Object Model)
keywords: vbob6.chm1092849
f1_keywords:
- vbob6.chm1092849
ms.prod: office
ms.assetid: 2482995e-ca97-067c-a7ae-cbeca2113199
ms.date: 12/06/2018
---


# ReferencesEvents property (VBA Add-In Object Model)

Returns the **ReferencesEvents** object. Read-only.

### Settings

The setting for the [argument](../../Glossary/vbe-glossary.md#argument) you pass to the **ReferencesEvents** property is:

|**Argument**|**Description**|
|:-----|:-----|
| _vbproject_|If  _vbproject_ points to **Nothing**, the object that is returned will supply events for the **References** collections of all **VBProject** objects in the **VBProjects** collection. If  _vbproject_ points to a valid **[VBProject](vbproject-object-vba-add-in-object-model.md)** object, the object that is returned will supply events for only the **References** collection for that [project](../../Glossary/vbe-glossary.md#project).|

### Remarks

The **ReferencesEvents** property takes an argument and returns an [event source object](../../Glossary/vbe-glossary.md#event-source-object). The **ReferencesEvents** object is the source for events that are triggered when references are added or removed.

### See also

- [Collections (Visual Basic Add-In Model)](../visual-basic-add-in-model/collections-visual-basic-add-in-model.md)
- [Visual Basic Add-in Model reference](visual-basic-add-in-model-reference.md)
- [Visual Basic language reference](visual-basic-language-reference.md)