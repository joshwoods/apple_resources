

- AppKit
- NSGridView
-  init(frame:) 

Initializer

# init(frame:)

Creates a newly allocated grid view object with the specified frame rectangle.

macOS 10.12+

``` source
@MainActor
init(frame frameRect: NSRect)
```

## Parameters 

`frameRect`  

The frame rectangle for the view, measured in points. The origin of the frame is relative to the superview in which you plan to add it.

## See Also

### Creating a Grid View

convenience init(numberOfColumns: Int, rows: Int)

Creates a newly allocated grid view object with the specified number of columns and rows.

convenience init(views: [[NSView]])

Creates a newly allocated grid view object with the specified array of arrays of views.

init?(coder: NSCoder)

Creates a newly allocated grid view object from the coder.

