

- SwiftUI
- EdgeInsets3D
-  init(horizontal:vertical:depth:) 

Initializer

# init(horizontal:vertical:depth:)

Creates an `EdgeInsets3D` value with values provided for each axis.

visionOS 1.0+

``` source
init(
    horizontal: CGFloat = 0,
    vertical: CGFloat = 0,
    depth: CGFloat = 0
)
```

## Parameters 

`horizontal`  

The insets to apply along the horizontal axis.

`vertical`  

The insets to apply along the vertical axis.

`depth`  

The insets to apply along the depth axis.

## See Also

### Creating an edge inset

init(top: CGFloat, leading: CGFloat, bottom: CGFloat, trailing: CGFloat, front: CGFloat, back: CGFloat)

Creates an `EdgeInsets3D` value with values provided for each face.

