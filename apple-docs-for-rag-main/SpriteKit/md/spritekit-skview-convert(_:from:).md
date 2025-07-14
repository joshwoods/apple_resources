

- SpriteKit
- SKView
-  convert(\_:from:) 

Instance Method

# convert(\_:from:)

Converts a point from scene coordinates to view coordinates.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
func convert(
    _ point: CGPoint,
    from scene: SKScene
) -> CGPoint
```

## Parameters 

`point`  

A point in scene coordinates.

`scene`  

A scene.

## Return Value

The same point in the view’s coordinate system.

## Discussion

This method performs the coordinate conversion as if the scene is presented inside the view.

## See Also

### Converting Between View and Scene Coordinates

func convert(CGPoint, to: SKScene) -> CGPoint

Converts a point from view coordinates to scene coordinates.

