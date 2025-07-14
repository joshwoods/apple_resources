

- PencilKit
-  PKLassoTool 

Structure

# PKLassoTool

A tool for selecting stroked lines and shapes in a canvas view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
struct PKLassoTool
```

## Overview

A PKLassoTool object supports the selection of content on a PKCanvasView. When active, the canvas uses incoming touch events to determine what content to add to the selection.

Create a lasso tool programmatically or display a PKToolPicker object from which the user selects the tool. Assign the resulting object to the tool property of your PKCanvasView object. The canvas uses any subsequent touch sequences to select content on the canvas.

## Topics

### Creating a lasso tool

init()

Creates a lasso tool for selecting content on a canvas view.

### Using reference types

class PKLassoToolReference

A tool for selecting stroked lines and shapes in a canvas view.

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

struct PKEraserTool

A tool for erasing previously drawn content in a canvas view.

protocol PKTool

An interface adopted by drawing and writing tools used by a canvas view.

