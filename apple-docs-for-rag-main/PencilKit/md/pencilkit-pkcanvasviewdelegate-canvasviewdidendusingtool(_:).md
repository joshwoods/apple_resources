

- PencilKit
- PKCanvasViewDelegate
-  canvasViewDidEndUsingTool(\_:) 

Instance Method

# canvasViewDidEndUsingTool(\_:)

Tells the delegate that the user ended a drawing sequence with the tool they were using.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func canvasViewDidEndUsingTool(_ canvasView: PKCanvasView)
```

## Parameters 

`canvasView`  

The canvas view whose contents changed.

## See Also

### Responding to new event sequences

func canvasViewDidBeginUsingTool(PKCanvasView)

Tells the delegate that the user started a new drawing sequence with the currently selected tool.

