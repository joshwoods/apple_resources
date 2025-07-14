

- SpriteKit
- SKPhysicsJointSliding
-  shouldEnableLimits 

Instance Property

# shouldEnableLimits

A Boolean value that indicates whether the sliding joint is restricted so that the objects may only slide a finite distance from the initial anchor point.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var shouldEnableLimits: Bool { get set }
```

## Discussion

The default value is false. If true, then the lowerDistanceLimit and upperDistanceLimit properties are used to limit the distance of the sliding joint.

## See Also

### Configuring a Sliding Joint

var lowerDistanceLimit: CGFloat

The smallest distance allowed for the sliding joint.

var upperDistanceLimit: CGFloat

The largest distance allowed for the sliding joint.

