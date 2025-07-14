

- PencilKit
-  PKCanvasViewDrawingPolicy 

Enumeration

# PKCanvasViewDrawingPolicy

Constants that you use to specify the type of drawing gestures your app permits while the user draws on the canvas.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
enum PKCanvasViewDrawingPolicy
```

## Topics

### Drawing policies

case `default`

The default input type to use for drawing on a canvas.

case anyInput

Allows drawing on the canvas from any input source.

case pencilOnly

Pencil touches are the only input that draw on the canvas.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the drawing environment

var tool: any PKTool

The currently selected tool used for drawing.

var isRulerActive: Bool

A Boolean value that indicates whether a ruler view is visible on the canvas.

var allowsFingerDrawing: Bool

A Boolean value that indicates whether the canvas accepts input from the user’s finger in addition to Apple Pencil.

Deprecated

var drawingPolicy: PKCanvasViewDrawingPolicy

The policy that controls the types of touches allowed when drawing on the canvas.

