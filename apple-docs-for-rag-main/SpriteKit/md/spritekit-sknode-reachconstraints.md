

- SpriteKit
- SKNode
-  reachConstraints 

Instance Property

# reachConstraints

The reach constraints to apply to the node when executing a reach action.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
@NSCopying
var reachConstraints: SKReachConstraints? { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@NSCopying @MainActor
var reachConstraints: SKReachConstraints? { get set }
```

## Discussion

To use inverse kinematics, create a new SKReachConstraints object and assign it to this property. When a reach action calculates the new positions of this node, the possible values for this node are restricted to the constraints defined by this object. For more information on the inverse kinematic actions, see SKAction.

## See Also

### Constraining Node Position or Rotation

var constraints: [SKConstraint]?

A list of constraints to apply to the node.

