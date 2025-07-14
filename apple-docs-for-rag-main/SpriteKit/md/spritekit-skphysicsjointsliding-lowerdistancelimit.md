

- SpriteKit
- SKPhysicsJointSliding
-  lowerDistanceLimit 

Instance Property

# lowerDistanceLimit

The smallest distance allowed for the sliding joint.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var lowerDistanceLimit: CGFloat { get set }
```

## Discussion

The default value is `0.0`.

## See Also

### Configuring a Sliding Joint

var shouldEnableLimits: Bool

A Boolean value that indicates whether the sliding joint is restricted so that the objects may only slide a finite distance from the initial anchor point.

var upperDistanceLimit: CGFloat

The largest distance allowed for the sliding joint.

