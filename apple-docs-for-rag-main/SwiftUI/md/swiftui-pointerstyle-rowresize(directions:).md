

- SwiftUI
- PointerStyle
-  rowResize(directions:) 

Type Method

# rowResize(directions:)

The pointer style for resizing a row, or horizontal division.

macOS 15.0+

``` source
static func rowResize(directions: VerticalDirection.Set) -> PointerStyle
```

## Parameters 

`directions`  

The vertical directions in which a row can be resized.

## Discussion

You may apply this pointer style to a single view or a view hierarchy using the pointerStyle(_:) modifier.

