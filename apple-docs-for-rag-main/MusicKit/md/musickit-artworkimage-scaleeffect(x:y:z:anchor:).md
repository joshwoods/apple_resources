

- MusicKit
- ArtworkImage
-  scaleEffect(x:y:z:anchor:) 

Instance Method

# scaleEffect(x:y:z:anchor:)

Scales this view by the specified horizontal, vertical, and depth factors.

MusicKitSwiftUIvisionOS 1.0+

``` source
nonisolated
func scaleEffect(
    x: CGFloat = 1.0,
    y: CGFloat = 1.0,
    z: CGFloat = 1.0,
    anchor: UnitPoint3D = .center
) -> some View
```

## Parameters 

`x`  

The horizontal scale factor for this view.

`y`  

The vertical scale factor for this view.

`z`  

The depth scale factor for this view.

`anchor`  

The anchor point about which to scale the view. Defaults to center.

## Return Value

A view that scales this view by `x`,`y`, and `z`.

## Discussion

The original dimensions of the view are considered to be unchanged by scaling the contents. To change the dimensions of the view, use a modifier like `frame()` instead.

