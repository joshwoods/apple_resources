

- UIKit
- UIView
-  convert(\_:to:) 

Instance Method

# convert(\_:to:)

Converts a rectangle from the receiver’s coordinate system to that of another view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func convert(
    _ rect: CGRect,
    to view: UIView?
) -> CGRect
```

## Parameters 

`rect`  

A rectangle specified in the local coordinate system (bounds) of the receiver.

`view`  

The view that is the target of the conversion operation. If `view` is `nil`, this method instead converts to window base coordinates. Otherwise, both `view` and the receiver must belong to the same UIWindow object.

## Return Value

The converted rectangle.

## See Also

### Converting between view coordinate systems

func convert(CGPoint, to: UIView?) -> CGPoint

Converts a point from the receiver’s coordinate system to that of the specified view.

func convert(CGPoint, from: UIView?) -> CGPoint

Converts a point from the coordinate system of a given view to that of the receiver.

func convert(CGRect, from: UIView?) -> CGRect

Converts a rectangle from the coordinate system of another view to that of the receiver.

