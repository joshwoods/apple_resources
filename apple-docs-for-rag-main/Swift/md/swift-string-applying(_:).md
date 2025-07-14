

- Swift
- String
-  applying(\_:) 

Instance Method

# applying(\_:)

Applies the given difference to this collection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

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

## See Also

### Creating and Applying Differences

func difference&lt;C>(from: C) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection.

func difference&lt;C>(from: C, by: (C.Element, Self.Element) -> Bool) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection, using the given predicate as an equivalence test.

