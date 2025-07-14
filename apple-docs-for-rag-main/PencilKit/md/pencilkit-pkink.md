

- PencilKit
-  PKInk 

Structure

# PKInk

A structure that represents an ink that specifies its type, color, and width.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
struct PKInk
```

## Mentioned in 

Supporting backward compatibility for ink types

## Topics

### Creating an ink object

init(PKInk.InkType, color: UIColor)

Creates a new ink, specifying its type and color.

init(PKInk.InkType, color: NSColor)

Creates a new ink, specifying its type and color.

typealias InkType

A type alias referring to the ink type of an inking tool.

### Getting the ink attributes

var color: UIColor

The color of this ink.

var color: NSColor

The color of this ink.

var inkType: PKInk.InkType

The line presentation to use for this Ink.

### Supporting backward compatibility

var requiredContentVersion: PKContentVersion

The version of PencilKit necessary to use the ink.

### Using reference types

class PKInkReference

Provides a description of the creation and rendering of marks on a canvas.

## Relationships

### Conforms To

- Copyable

## See Also

### Canvas

Drawing with PencilKit

Add expressive, low-latency drawing to your app using PencilKit.

Customizing Scribble with Interactions

Enable writing on a non-text-input view by adding interactions.

Inspecting, Modifying, and Constructing PencilKit Drawings

Score users’ ability to match PencilKit drawings generated from text, by accessing the strokes and points inside PencilKit drawings.

class PKCanvasView

A view that captures Apple Pencil input and displays the rendered results in an iOS app.

struct PKDrawing

A structure representing the drawing information captured by a canvas view.

struct PKStroke

A structure that represents the paths, boundaries, and other properties of a stroke drawn on a canvas.

struct PKStrokePath

A structure that captures the components of a stroke and provides methods to find and interpolate points along the stroke’s path.

struct PKStrokePoint

A structure that represents the properties of a specific point along a stroke’s path.

