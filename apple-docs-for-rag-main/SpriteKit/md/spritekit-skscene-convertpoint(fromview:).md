

- SpriteKit
- SKScene
-  convertPoint(fromView:) 

Instance Method

# convertPoint(fromView:)

Converts a point from view coordinates to scene coordinates.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
func convertPoint(fromView point: CGPoint) -> CGPoint
```

## Parameters 

`point`  

A point in view coordinates.

## Return Value

The same point in the scene’s coordinate system.

## Discussion

The scene must be presented in a view before calling this method.

## See Also

### Converting Between Coordinate Systems

func convertPoint(toView: CGPoint) -> CGPoint

Converts a point from scene coordinates to view coordinates.

