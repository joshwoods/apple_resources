

- Foundation
- NSArray
-  shuffled(using:) 

Instance Method

# shuffled(using:)

Returns a new array that lists this array’s elements in a random order, using the specified random source.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func shuffled(using randomSource: GKRandomSource) -> [Any]
```

## Parameters 

`randomSource`  

A GameplayKit random source object.

## Return Value

A new array that lists this array’s elements in a random order.

## Discussion

Use the `randomSource` parameter to influence the random shuffling. For example, to reproduce a series of shuffles for testing, you can create a GKARC4RandomSource object using the seed value of a previously used random source.

This method is equivalent to the GKRandomSource method arrayByShufflingObjects(in:), but as an NSArray method it preserves generic type parameters.

## See Also

### Randomly Shuffling an Array

func shuffled() -> [Any]

Returns a new array that lists this array’s elements in a random order.

