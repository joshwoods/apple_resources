

- AppKit
- NSGridView
-  init(numberOfColumns:rows:) 

Initializer

# init(numberOfColumns:rows:)

Creates a newly allocated grid view object with the specified number of columns and rows.

macOS 10.12+

``` source
@MainActor
convenience init(
    numberOfColumns columnCount: Int,
    rows rowCount: Int
)
```

## Parameters 

`columnCount`  

The number of columns for this grid view.

`rowCount`  

The number of rows for this grid view.

## See Also

### Creating a Grid View

convenience init(views: [[NSView]])

Creates a newly allocated grid view object with the specified array of arrays of views.

init(frame: NSRect)

Creates a newly allocated grid view object with the specified frame rectangle.

init?(coder: NSCoder)

Creates a newly allocated grid view object from the coder.

