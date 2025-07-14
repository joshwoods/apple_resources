

- RealityKit
- PhysicsJoints
-  applying(\_:) 

Instance Method

# applying(\_:)

Applies the given difference to this collection.

RealityKitSwiftiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func applying(_ difference: CollectionDifference) -> Self?
```

## Parameters 

`difference`  

The difference to be applied.

## Return Value

An instance representing the state of the receiver with the difference applied, or `nil` if the difference is incompatible with the receiver’s state.

## Discussion

Complexity

O(*n* + *c*), where *n* is `self.count` and *c* is the number of changes contained by the parameter.

