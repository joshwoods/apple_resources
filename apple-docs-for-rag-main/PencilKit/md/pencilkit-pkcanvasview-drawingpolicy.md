

- PencilKit
- PKCanvasView
-  drawingPolicy 

Instance Property

# drawingPolicy

The policy that controls the types of touches allowed when drawing on the canvas.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var drawingPolicy: PKCanvasViewDrawingPolicy { get set }
```

## See Also

### Configuring the drawing environment

var tool: any PKTool

The currently selected tool used for drawing.

var isRulerActive: Bool

A Boolean value that indicates whether a ruler view is visible on the canvas.

var allowsFingerDrawing: Bool

A Boolean value that indicates whether the canvas accepts input from the user’s finger in addition to Apple Pencil.

Deprecated

enum PKCanvasViewDrawingPolicy

Constants that you use to specify the type of drawing gestures your app permits while the user draws on the canvas.

