

- GameplayKit
- GKBehavior
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the weight associated with the goal specified by subscript syntax.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
subscript(goal: GKGoal) -> NSNumber! { get set }
```

## Parameters 

`goal`  

A goal already included in the behavior’s set of goals.

## Return Value

The weight to be applied to the goal’s influence on an agent’s speed and direction, or `0.0` if the goal is not in the behavior.

## Discussion

This method is equivalent to the weight(for:) method, but allows access using subscript syntax.

## See Also

### Working with Goals Using Subscript Syntax

subscript(Int) -> GKGoal

Returns the goal at the specified index in the behavior’s list of goals.

