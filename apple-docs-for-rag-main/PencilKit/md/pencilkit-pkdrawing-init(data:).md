

- PencilKit
- PKDrawing
-  init(data:) 

Initializer

# init(data:)

Creates a drawing object and populates it with previously drawn content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
init(data: Data) throws
```

## Parameters 

`data`  

The initial data to add to the canvas. Only specify data you previously obtained from a canvas view.

## Discussion

This initializer creates a new canvas object initialized with the specified data.

## See Also

### Creating a drawing object

init&lt;S>(strokes: S)

Creates a drawing object and populates it with a sequence of strokes the user provides.

init()

Creates an empty drawing object.

