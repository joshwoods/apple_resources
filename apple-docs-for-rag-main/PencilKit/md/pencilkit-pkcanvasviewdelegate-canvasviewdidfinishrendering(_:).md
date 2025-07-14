

- PencilKit
- PKCanvasViewDelegate
-  canvasViewDidFinishRendering(\_:) 

Instance Method

# canvasViewDidFinishRendering(\_:)

Tells the delegate that the previously drawn content is ready to display.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func canvasViewDidFinishRendering(_ canvasView: PKCanvasView)
```

## Parameters 

`canvasView`  

The canvas view whose contents changed.

## Discussion

The PKCanvasView object calls this method when you assign a new drawing to its drawing property, when the user zooms in on the canvas, or when the canvas scrolls.

## See Also

### Responding to drawing-related changes

func canvasViewDrawingDidChange(PKCanvasView)

Tells the delegate that the contents of the current drawing changed.

