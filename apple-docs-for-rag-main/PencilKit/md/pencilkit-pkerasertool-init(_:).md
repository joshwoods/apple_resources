

- PencilKit
- PKEraserTool
-  init(\_:) 

Initializer

# init(\_:)

Creates an eraser tool object that removes objects wholly or partially from a canvas view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
init(_ eraserType: PKEraserTool.EraserType)
```

## Parameters 

`eraserType`  

A constant that determines how the eraser affects drawn content. For a list of possible values, see PKEraserTool.EraserType.

## Discussion

This initializer creates a new eraser tool object.

## See Also

### Creating an eraser tool

init(PKEraserTool.EraserType, width: CGFloat)

Creates an eraser tool object with the specified width.

