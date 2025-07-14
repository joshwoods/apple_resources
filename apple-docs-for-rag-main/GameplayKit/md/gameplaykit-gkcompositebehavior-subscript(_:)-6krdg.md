

- GameplayKit
- GKCompositeBehavior
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the individual behavior at the specified index in the composite behavior’s list of behaviors.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
subscript(idx: Int) -> GKBehavior { get }
```

## Parameters 

`idx`  

An index in the composite behavior’s list of individual behaviors; it must be less than the value of the behaviorCount property.

## Return Value

The behavior at the specified index.

## Discussion

The order of individual behaviors in a composite behavior is undefined. However, you can use this method to enumerate all individual behaviors in a composite behavior.

## See Also

### Working with Behaviors Using Subscript Syntax

subscript(GKBehavior) -> NSNumber

Returns the weight associated with the behavior specified by subscript syntax.

