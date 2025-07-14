

- AppKit
- NSCursor
-  rowResize(directions:) 

Type Method

# rowResize(directions:)

Returns the cursor for resizing a row (horizontal divider) in the specified direction.

Mac Catalyst 18.0+macOS 15.0+

``` source
class func rowResize(directions: NSVerticalDirection.Set) -> NSCursor
```

## Parameters 

`directions`  

The directions in which a row can be resized. This must not be empty.

