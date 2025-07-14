

- PencilKit
- PKDrawing
-  init(strokes:) 

Initializer

# init(strokes:)

Creates a drawing object and populates it with a sequence of strokes the user provides.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(strokes: S) where S : Sequence, S.Element == PKStroke
```

## Parameters 

`strokes`  

A sequence of PKStroke elements.

## See Also

### Creating a drawing object

init(data: Data) throws

Creates a drawing object and populates it with previously drawn content.

init()

Creates an empty drawing object.

