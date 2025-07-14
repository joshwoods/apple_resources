

- UIKit
- UIView
-  convert(\_:to:) 

Instance Method

# convert(\_:to:)

Converts a point from the receiver’s coordinate system to that of the specified view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func convert(
    _ point: CGPoint,
    to view: UIView?
) -> CGPoint
```

## Parameters 

`point`  

A point specified in the local coordinate system (bounds) of the receiver.

`view`  

The view into whose coordinate system `point` is to be converted. If `view` is `nil`, this method instead converts to window base coordinates. Otherwise, both `view` and the receiver must belong to the same UIWindow object.

## Return Value

The point converted to the coordinate system of `view`.

## See Also

### Converting between view coordinate systems

func convert(CGPoint, from: UIView?) -> CGPoint

Converts a point from the coordinate system of a given view to that of the receiver.

func convert(CGRect, to: UIView?) -> CGRect

Converts a rectangle from the receiver’s coordinate system to that of another view.

func convert(CGRect, from: UIView?) -> CGRect

Converts a rectangle from the coordinate system of another view to that of the receiver.

