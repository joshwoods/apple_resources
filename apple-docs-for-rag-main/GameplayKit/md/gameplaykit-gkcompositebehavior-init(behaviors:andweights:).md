

- GameplayKit
- GKCompositeBehavior
-  init(behaviors:andWeights:) 

Initializer

# init(behaviors:andWeights:)

Creates a behavior with the specified behaviors and weights.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    behaviors: [GKBehavior],
    andWeights weights: [NSNumber]
)
```

## Parameters 

`behaviors`  

An array of behavior objects.

`weights`  

An array of numbers, each of which is the weight to be applied to the behavior at the corresponding index in the `behaviors` array.

## Return Value

A new behavior object. To assign a behavior to an agent, use the agent’s behavior property.

## See Also

### Creating a Composite Behavior

convenience init(behaviors: [GKBehavior])

Creates a composite behavior from the specified individual behaviors.

