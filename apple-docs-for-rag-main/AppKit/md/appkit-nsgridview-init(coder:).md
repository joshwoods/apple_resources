

- AppKit
- NSGridView
-  init(coder:) 

Initializer

# init(coder:)

Creates a newly allocated grid view object from the coder.

macOS 10.12+

``` source
@MainActor
init?(coder: NSCoder)
```

## Parameters 

`coder`  

The coder object.

## See Also

### Creating a Grid View

convenience init(numberOfColumns: Int, rows: Int)

Creates a newly allocated grid view object with the specified number of columns and rows.

convenience init(views: [[NSView]])

Creates a newly allocated grid view object with the specified array of arrays of views.

init(frame: NSRect)

Creates a newly allocated grid view object with the specified frame rectangle.

