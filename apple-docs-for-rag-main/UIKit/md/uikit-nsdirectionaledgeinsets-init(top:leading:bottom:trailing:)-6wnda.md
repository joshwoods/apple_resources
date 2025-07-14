

- UIKit
- NSDirectionalEdgeInsets
-  init(top:leading:bottom:trailing:) 

Initializer

# init(top:leading:bottom:trailing:)

Creates a directional edge insets structure that contains the specified values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

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

init(EdgeInsets)

Creates a directional edge insets structure from a SwiftUI edge insets structure.

