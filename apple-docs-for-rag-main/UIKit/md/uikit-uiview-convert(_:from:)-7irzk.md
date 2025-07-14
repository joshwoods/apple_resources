

- UIKit
- UIView
-  convert(\_:from:) 

Instance Method

# convert(\_:from:)

Converts a rectangle from the coordinate system of another view to that of the receiver.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func convert(
    _ rect: CGRect,
    from view: UIView?
) -> CGRect
```

## Parameters 

`rect`  

A rectangle specified in the local coordinate system (bounds) of `view`.

`view`  

The view with `rect` in its coordinate system. If `view` is `nil`, this method instead converts from window base coordinates. Otherwise, both `view` and the receiver must belong to the same UIWindow object.

## Return Value

The converted rectangle.

## See Also

### Converting between view coordinate systems

func convert(CGPoint, to: UIView?) -> CGPoint

Converts a point from the receiver’s coordinate system to that of the specified view.

func convert(CGPoint, from: UIView?) -> CGPoint

Converts a point from the coordinate system of a given view to that of the receiver.

func convert(CGRect, to: UIView?) -> CGRect

Converts a rectangle from the receiver’s coordinate system to that of another view.

