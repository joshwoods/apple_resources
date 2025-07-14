

- GameplayKit
- GKCompositeBehavior
-  init(behaviors:) 

Initializer

# init(behaviors:)

Creates a composite behavior from the specified individual behaviors.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(behaviors: [GKBehavior])
```

## Parameters 

`behaviors`  

An array of behavior objects.

## Return Value

A new behavior object. To assign a behavior to an agent, use the agent’s behavior property.

## Discussion

The new behavior contains the specified behaviors, each with a weight of `1.0`. To change an individual behavior’s weight after creating the composite behavior, keep a reference to that behavior and use the setWeight(_:for:) method.

For more information, see GameplayKit Programming Guide.

## See Also

### Creating a Composite Behavior

convenience init(behaviors: [GKBehavior], andWeights: [NSNumber])

Creates a behavior with the specified behaviors and weights.

