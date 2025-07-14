

- GameplayKit
- GKCompositeBehavior
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the weight associated with the behavior specified by subscript syntax.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
subscript(behavior: GKBehavior) -> NSNumber { get set }
```

## Parameters 

`behavior`  

An individual behavior already included in the composite behavior’s set of behaviors.

## Return Value

The weight applied to that behavior’s influence on an agent’s speed and direction, or `0.0` if that behavior is not in the composite behavior.

## Discussion

This method is equivalent to the weight(for:) method, but allows access using subscript syntax.

## See Also

### Working with Behaviors Using Subscript Syntax

subscript(Int) -> GKBehavior

Returns the individual behavior at the specified index in the composite behavior’s list of behaviors.

