

- UIKit
- NSLayoutYAxisAnchor
-  anchorWithOffset(to:) 

Instance Method

# anchorWithOffset(to:)

Creates a layout dimension object from two anchors.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
func anchorWithOffset(to otherAnchor: NSLayoutYAxisAnchor) -> NSLayoutDimension
```

## Parameters 

`otherAnchor`  

The second anchor to use when creating the layout dimension.

## Return Value

The NSLayoutDimension object represented by the two anchors.

## Discussion

Use the returned object to define constraints relative to the space between the current anchor and the object in the `otherAnchor` parameter.

