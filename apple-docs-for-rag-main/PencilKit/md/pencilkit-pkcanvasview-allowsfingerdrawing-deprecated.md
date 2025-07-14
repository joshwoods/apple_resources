

- PencilKit
- PKCanvasView
-  allowsFingerDrawing Deprecated

Instance Property

# allowsFingerDrawing

A Boolean value that indicates whether the canvas accepts input from the user’s finger in addition to Apple Pencil.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var allowsFingerDrawing: Bool { get set }
```

Deprecated

Use drawingPolicy instead.

## See Also

### Configuring the drawing environment

var tool: any PKTool

The currently selected tool used for drawing.

var isRulerActive: Bool

A Boolean value that indicates whether a ruler view is visible on the canvas.

var drawingPolicy: PKCanvasViewDrawingPolicy

The policy that controls the types of touches allowed when drawing on the canvas.

enum PKCanvasViewDrawingPolicy

Constants that you use to specify the type of drawing gestures your app permits while the user draws on the canvas.

