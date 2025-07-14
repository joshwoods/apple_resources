

- PencilKit
- PKDrawingReference
-  init(data:) 

Initializer

# init(data:)

Creates a drawing object and populates it with previously drawn content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
init(data: Data) throws
```

## Parameters 

`data`  

The initial data to add to the canvas. Only specify data you previously obtained from a canvas view.

## Return Value

A new canvas object initialized with the specified data.

## See Also

### Creating a drawing object

convenience init(strokes: [PKStroke])

Creates a drawing object with the strokes you supply.

init()

Creates an empty drawing object.

