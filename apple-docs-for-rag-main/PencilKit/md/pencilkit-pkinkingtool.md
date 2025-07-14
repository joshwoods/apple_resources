

- PencilKit
-  PKInkingTool 

Structure

# PKInkingTool

A structure that defines the drawing characteristics (width, color, pen style) to use when drawing lines on a canvas view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
struct PKInkingTool
```

## Mentioned in 

Supporting backward compatibility for ink types

## Overview

A PKInkingTool object supports the creation of new content on a PKCanvasView. With an inking tool, the canvas turns touch input from the user into a continuously rendered stroke. The value in the width property determines the base width of that stroke; however, that base value also depends on input from Apple Pencil, including force, azimuth, and angle data.

Create an inking tool programmatically, or display a PKToolPicker object and from which a user can select a tool. Assign the resulting object to the tool property of your PKCanvasView object. The canvas uses any subsequent touch sequences to draw new content on the canvas. Assigning a new inking tool doesn’t change the characteristics for any previously drawn strokes.

## Topics

### Creating an inking tool

init(PKInkingTool.InkType, color: UIColor, width: CGFloat?)

Creates an ink tool object with the specified color and line width values.

init(PKInkingTool.InkType, color: NSColor, width: CGFloat?)

Creates an ink tool object with the specified color and line width values.

init(ink: PKInk, width: CGFloat)

Create an inking tool with the specified ink and width.

### Getting the width information

var defaultWidth: CGFloat

The default line width for the specified tool type.

var validWidthRange: ClosedRange&lt;CGFloat>

The range of widths allowed for an ink of this type.

### Getting the inking tool attributes

var color: UIColor

The color of the ink.

var color: NSColor

The color of the ink.

var width: CGFloat

The width of the ink.

var ink: PKInk

The ink used by this inking tool.

### Getting the tool type

var inkType: PKInkingTool.InkType

The tool type that determines the shape of the rendered content.

enum InkType

The type that defines the shape of stroked lines.

### Working with colors

static func convertColor(UIColor, from: UIUserInterfaceStyle, to: UIUserInterfaceStyle) -> UIColor

Convert a color from one user interface style to another.

### Supporting backward compatibility

var requiredContentVersion: PKContentVersion

The version of PencilKit necessary to use the inking tool.

### Using reference types

class PKInkingToolReference

An object that defines the drawing characteristics (width, color, pen style) to use when drawing lines on a canvas view.

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

struct PKEraserTool

A tool for erasing previously drawn content in a canvas view.

struct PKLassoTool

A tool for selecting stroked lines and shapes in a canvas view.

protocol PKTool

An interface adopted by drawing and writing tools used by a canvas view.

