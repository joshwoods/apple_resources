

- AppKit
- NSLayoutXAxisAnchor
-  anchorWithOffset(to:) 

Instance Method

# anchorWithOffset(to:)

Creates a layout dimension object from two anchors.

macOS 10.12+

``` source
func anchorWithOffset(to otherAnchor: NSLayoutXAxisAnchor) -> NSLayoutDimension
```

## Parameters 

`otherAnchor`  

The second anchor to use when creating the layout dimension.

## Return Value

The NSLayoutDimension object represented by the two anchors.

## Discussion

Use the returned object to define constraints relative to the space between the current anchor and the object in the `otherAnchor` parameter.

