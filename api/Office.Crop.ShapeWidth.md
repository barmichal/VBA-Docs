---
title: Crop.ShapeWidth Property (Office)
ms.prod: office
api_name:
- Office.Crop.ShapeWidth
ms.assetid: 4ee0ec53-1da8-b981-ec03-bb0ce4b616da
ms.date: 06/08/2017
---


# Crop.ShapeWidth Property (Office)

Gets or sets the width of a shape that is used to crop an image. Read/write


## Syntax

 _expression_. `ShapeWidth`

 _expression_ An expression that returns a [Crop](./Office.Crop.md) object.


## Return value

Single


## Example

The following example inserts a 200 x 200 image into a PowerPoint presentation approximately in the center of the slide. It then resizes the image inside the frame to 100 x 100. The image frame stays at 200 x 200. The code then adds a square (the default shape) just above and to the right of the image, essentially cropping the lower left corner of the image.


```vb
Sub CropImage() 
 ActivePresentation.Slides(1).Shapes.AddPicture "c:\myImage.png", msoFalse, msoTrue, 250,150, 200, 200 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.PictureHeight = 100 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.PictureWidth = 100 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.PictureOffsetX = 0 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.PictureOffsetY = 0 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.ShapeHeight = 100 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.ShapeWidth = 100 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.ShapeLeft = 330 
 ActivePresentation.Slides(1).Shapes(1).PictureFormat.Crop.ShapeTop = 170 
End Sub 

```


## See also


[Crop Object](Office.Crop.md)



[Crop Object Members](./overview/Library-Reference/crop-members-office.md)

