

- PencilKit
- PKCanvasViewDelegate
-  canvasViewDrawingDidChange(\_:) 

Instance Method

# canvasViewDrawingDidChange(\_:)

Tells the delegate that the contents of the current drawing changed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func canvasViewDrawingDidChange(_ canvasView: PKCanvasView)
```

## Parameters 

`canvasView`  

The canvas view whose contents changed.

## See Also

### Responding to drawing-related changes

func canvasViewDidFinishRendering(PKCanvasView)

Tells the delegate that the previously drawn content is ready to display.

