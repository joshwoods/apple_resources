

- SwiftUI
- PointerStyle
-  shape(\_:eoFill:size:) 

Type Method

# shape(\_:eoFill:size:)

Initializes a pointer style with a given shape.

visionOS 2.0+

``` source
static func shape(
    _ shape: some Shape,
    eoFill: Bool = false,
    size: CGSize
) -> PointerStyle
```

## Parameters 

`shape`  

The pointer shape.

`eoFill`  

A Boolean that indicates whether the shape is interpreted with the even-odd winding number rule.

`size`  

The size of the pointer shape.

## Discussion

For guidance on using a custom pointer, refer to Pointing devices in the Human Interface Guidelines.

You may apply this pointer style to a single view or a view hierarchy using the pointerStyle(_:) modifier.

