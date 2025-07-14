

- PencilKit
- PKEraserToolReference
-  init(eraserType:) 

Initializer

# init(eraserType:)

Creates an eraser tool object that removes objects wholly or partially from a canvas view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
init(eraserType: __PKEraserType)
```

## Parameters 

`eraserType`  

A constant that determines how the eraser affects drawn content. For a list of possible values, see PKEraserType.

## Return Value

A new eraser tool object.

## See Also

### Creating an eraser tool

init(eraserType: __PKEraserType, width: CGFloat)

