

- AppKit
- NSGridView
-  init(views:) 

Initializer

# init(views:)

Creates a newly allocated grid view object with the specified array of arrays of views.

macOS 10.12+

``` source
@MainActor
convenience init(views rows: [[NSView]])
```

## Parameters 

`rows`  

An array of arrays of grid view row objects.

## Discussion

This method creates an autoreleased grid view large enough to hold the passed array of rows. Each element in the array is itself an array of views for that row.

## See Also

### Creating a Grid View

convenience init(numberOfColumns: Int, rows: Int)

Creates a newly allocated grid view object with the specified number of columns and rows.

init(frame: NSRect)

Creates a newly allocated grid view object with the specified frame rectangle.

init?(coder: NSCoder)

Creates a newly allocated grid view object from the coder.

