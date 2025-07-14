

- PencilKit
-  PKEraserTool 

Structure

# PKEraserTool

A tool for erasing previously drawn content in a canvas view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
struct PKEraserTool
```

## Overview

A PKEraserTool object supports the deletion of content from a PKCanvasView object. The eraser tool’s type determines whether the canvas removes entire items or just the portion of an item that it touches.

Create an eraser tool programmatically or display a PKToolPicker object and let the user select the eraser. Assign the resulting object to the tool property of your PKCanvasView object. The canvas uses any subsequent touch sequences to erase content on the canvas.

## Topics

### Creating an eraser tool

init(PKEraserTool.EraserType)

Creates an eraser tool object that removes objects wholly or partially from a canvas view.

init(PKEraserTool.EraserType, width: CGFloat)

Creates an eraser tool object with the specified width.

### Getting the eraser type

var eraserType: PKEraserTool.EraserType

The behavior adopted by the eraser when deleting content.

enum EraserType

Constants that indicate the behavior of the eraser.

### Specifying the width

var width: CGFloat

The width of the eraser.

### Using reference types

class PKEraserToolReference

A tool for erasing previously drawn content in a canvas view.

## Relationships

### Conforms To

- Copyable
- Equatable
- PKTool

## See Also

### Tools

Configuring the PencilKit tool picker

Incorporate a custom PencilKit tool picker with a variety of system and custom tools into a drawing app.

class PKToolPicker

A tool palette that displays a selection of drawing tools and colors for tools that a person can choose from.

struct PKInkingTool

A structure that defines the drawing characteristics (width, color, pen style) to use when drawing lines on a canvas view.

struct PKLassoTool

A tool for selecting stroked lines and shapes in a canvas view.

protocol PKTool

An interface adopted by drawing and writing tools used by a canvas view.

