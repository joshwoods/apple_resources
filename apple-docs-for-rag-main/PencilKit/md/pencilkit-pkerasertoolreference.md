

- PencilKit
-  PKEraserToolReference 

Class

# PKEraserToolReference

A tool for erasing previously drawn content in a canvas view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class PKEraserToolReference
```

## Overview

A PKEraserTool object supports the deletion of content from a PKCanvasView object. The eraser tool’s type determines whether the canvas removes entire items or just the portion of an item that it touches.

Create an eraser tool programmatically or display a PKToolPicker object and let the user select the eraser. Assign the resulting object to the tool property of your PKCanvasView object. The canvas uses any subsequent touch sequences to erase content on the canvas.

## Topics

### Creating an eraser tool

init(eraserType: __PKEraserType)

Creates an eraser tool object that removes objects wholly or partially from a canvas view.

init(eraserType: __PKEraserType, width: CGFloat)

### Getting the eraser type

var eraserType: __PKEraserType

The behavior adopted by the eraser when deleting content.

### Getting the width information

var width: CGFloat

The width of the eraser.

class func defaultWidth(for: __PKEraserType) -> CGFloat

The default width for the specified eraser type.

class func minimumWidth(for: __PKEraserType) -> CGFloat

The minimum width for the specified eraser type.

class func maximumWidth(for: __PKEraserType) -> CGFloat

The maximum width for the specified eraser type.

## Relationships

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

