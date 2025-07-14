

- GameplayKit
- GKBehavior
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the goal at the specified index in the behavior’s list of goals.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
subscript(idx: Int) -> GKGoal { get }
```

## Parameters 

`idx`  

An index in the behavior’s list of goals; must be less than the value of the goalCount property.

## Return Value

The goal at the specified index.

## Discussion

The order of goals in a behavior is undefined. However, you can use this method to enumerate all goals in a behavior.

## See Also

### Working with Goals Using Subscript Syntax

subscript(GKGoal) -> NSNumber!

Returns the weight associated with the goal specified by subscript syntax.

