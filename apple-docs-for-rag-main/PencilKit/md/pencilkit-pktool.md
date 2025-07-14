

- PencilKit
-  PKTool 

Protocol

# PKTool

An interface adopted by drawing and writing tools used by a canvas view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
protocol PKTool
```

## Overview

Drawing and writing tools associated with a PKCanvasView adopt the PKTool protocol. Tools are user-facing, and the selected tool determines how the canvas interprets incoming gestures.

Don’t adopt this protocol in your own objects. Instead, create a tool object to provide users with the desired the tool behavior.

## Relationships

### Conforming Types

- PKEraserTool
- PKInkingTool
- PKLassoTool

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

struct PKLassoTool

A tool for selecting stroked lines and shapes in a canvas view.

