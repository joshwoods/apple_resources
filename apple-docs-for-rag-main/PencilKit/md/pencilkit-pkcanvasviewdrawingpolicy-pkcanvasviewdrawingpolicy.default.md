

- PencilKit
- PKCanvasViewDrawingPolicy
-  PKCanvasViewDrawingPolicy.default 

Case

# PKCanvasViewDrawingPolicy.default

The default input type to use for drawing on a canvas.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
case `default`
```

## Discussion

By default, if the tool picker is visible, respect the pencil interaction setting of the prefersPencilOnlyDrawing property; otherwise only accept input from Apple Pencil.

## See Also

### Drawing policies

case anyInput

Allows drawing on the canvas from any input source.

case pencilOnly

Pencil touches are the only input that draw on the canvas.

