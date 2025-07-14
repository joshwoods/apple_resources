

- UIKit
- UIEdgeInsets
-  init(top:left:bottom:right:) 

Initializer

# init(top:left:bottom:right:)

Creates an edge insets structure with the specified edges.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
init(
    top: CGFloat,
    left: CGFloat,
    bottom: CGFloat,
    right: CGFloat
)
```

## Parameters 

`top`  

The inset on the top of an object.

`left`  

The inset on the left of an object.

`bottom`  

The inset on the bottom of an object.

`right`  

The inset on the right of an object.

## Return Value

An initialized inset structure.

## Discussion

An inset is a margin around a rectangle. Positive values represent margins closer to the center of the rectangle, while negative values represent margins further from the center.

## See Also

### Creating edge insets

init()

Initializes the edge insets structure to default values.

