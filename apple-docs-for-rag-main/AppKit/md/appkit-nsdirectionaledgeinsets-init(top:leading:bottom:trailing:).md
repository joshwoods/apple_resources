

- AppKit
- NSDirectionalEdgeInsets
-  init(top:leading:bottom:trailing:) 

Initializer

# init(top:leading:bottom:trailing:)

Creates a directional edge insets structure that contains the specified values.

macOS 10.15+

``` source
init(
    top: CGFloat,
    leading: CGFloat,
    bottom: CGFloat,
    trailing: CGFloat
)
```

## Parameters 

`top`  

The inset on the top of an object.

`leading`  

The inset on the leading edge of an object. In a left-to-right system, the left edge is the leading edge. In a right-to-left system, the right edge is the leading edge.

`bottom`  

The inset on the bottom of an object.

`trailing`  

The inset on the trailing edge of an object. In a left-to-right system, the right edge is the trailing edge. In a right-to-left system, the left edge is the trailing edge.

## Return Value

An initialized inset structure.

## See Also

### Creating directional edge insets

init()

Creates a directional edge insets structure that contains default values.

