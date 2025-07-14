

- GameplayKit
- GKCompositeBehavior
-  behaviorCount 

Instance Property

# behaviorCount

The number of individual behaviors in the composite behavior.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var behaviorCount: Int { get }
```

## See Also

### Managing the Individual Behaviors in a Composite Behavior

func setWeight(Float, for: GKBehavior)

Sets the weight for the specified individual behavior’s influence on agents, adding that behavior to the composite behavior if it is not already present.

func weight(for: GKBehavior) -> Float

Returns the weight for the specified individual behavior’s influence on agents.

func remove(GKBehavior)

Removes the specified individual behavior from the composite behavior.

func removeAllBehaviors()

Removes all individual behaviors from the composite behavior.

