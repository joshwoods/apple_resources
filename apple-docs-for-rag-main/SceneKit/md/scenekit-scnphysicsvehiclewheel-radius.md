

- SceneKit
- SCNPhysicsVehicleWheel
-  radius 

Instance Property

# radius

The radius of the wheel.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var radius: CGFloat { get set }
```

## Discussion

When you create a wheel from a node, its default radius is half of the largest dimension of the node’s bounding box. (A wheel is always circular, even if the content of the node representing it is not.)

