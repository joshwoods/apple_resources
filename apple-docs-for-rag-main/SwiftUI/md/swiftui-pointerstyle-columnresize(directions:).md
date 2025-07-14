

- SwiftUI
- PointerStyle
-  columnResize(directions:) 

Type Method

# columnResize(directions:)

The pointer style for resizing a column, or vertical division.

macOS 15.0+

``` source
static func columnResize(directions: HorizontalDirection.Set) -> PointerStyle
```

## Parameters 

`directions`  

The horizontal directions in which a column can be resized. This must not be empty.

## Return Value

A pointer style for resizing a column.

## Discussion

You may apply this pointer style to a single view or a view hierarchy using the pointerStyle(_:) modifier.

