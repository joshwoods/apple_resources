

- SpriteKit
- SKView
-  convert(\_:to:) 

Instance Method

# convert(\_:to:)

Converts a point from view coordinates to scene coordinates.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
func convert(
    _ point: CGPoint,
    to scene: SKScene
) -> CGPoint
```

## Parameters 

`point`  

A point in view coordinates.

`scene`  

A scene.

## Return Value

The same point in the scene’s coordinate system.

## Discussion

This method performs the coordinate conversion as if the scene is presented inside the view.

## See Also

### Converting Between View and Scene Coordinates

func convert(CGPoint, from: SKScene) -> CGPoint

Converts a point from scene coordinates to view coordinates.

