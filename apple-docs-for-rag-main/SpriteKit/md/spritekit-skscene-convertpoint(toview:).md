

- SpriteKit
- SKScene
-  convertPoint(toView:) 

Instance Method

# convertPoint(toView:)

Converts a point from scene coordinates to view coordinates.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
func convertPoint(toView point: CGPoint) -> CGPoint
```

## Parameters 

`point`  

A point in scene coordinates.

## Return Value

The same point in the view’s coordinate system.

## Discussion

The scene must be presented in a view before calling this method.

## See Also

### Converting Between Coordinate Systems

func convertPoint(fromView: CGPoint) -> CGPoint

Converts a point from view coordinates to scene coordinates.

