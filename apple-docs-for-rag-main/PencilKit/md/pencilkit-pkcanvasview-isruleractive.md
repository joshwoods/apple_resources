

- PencilKit
- PKCanvasView
-  isRulerActive 

Instance Property

# isRulerActive

A Boolean value that indicates whether a ruler view is visible on the canvas.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isRulerActive: Bool { get set }
```

## See Also

### Configuring the drawing environment

var tool: any PKTool

The currently selected tool used for drawing.

var allowsFingerDrawing: Bool

A Boolean value that indicates whether the canvas accepts input from the user’s finger in addition to Apple Pencil.

Deprecated

var drawingPolicy: PKCanvasViewDrawingPolicy

The policy that controls the types of touches allowed when drawing on the canvas.

enum PKCanvasViewDrawingPolicy

Constants that you use to specify the type of drawing gestures your app permits while the user draws on the canvas.

