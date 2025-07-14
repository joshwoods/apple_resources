

- SpriteKit
- SKNode
-  constraints 

Instance Property

# constraints

A list of constraints to apply to the node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var constraints: [SKConstraint]? { get set }
```

**watchOS**

``` source
var constraints: [SKConstraint]? { get set }
```

## Discussion

Assign an array of SKConstraint objects to the node. The scene processes these constraints before the scene is rendered. The constraints are processed in array order. If multiple nodes in the node tree have constraints, there is no guaranteed order that the nodes are processed in.

## See Also

### Constraining Node Position or Rotation

var reachConstraints: SKReachConstraints?

The reach constraints to apply to the node when executing a reach action.

