

- AppKit
- NSCursor
-  columnResize(directions:) 

Type Method

# columnResize(directions:)

Returns the cursor for resizing a column (vertical divider) in the specified direction.

Mac Catalyst 18.0+macOS 15.0+

``` source
class func columnResize(directions: NSHorizontalDirection.Set) -> NSCursor
```

## Parameters 

`directions`  

The directions in which a column can be resized. This must not be empty.

