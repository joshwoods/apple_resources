

- Foundation
- NSArray
-  shuffled() 

Instance Method

# shuffled()

Returns a new array that lists this array’s elements in a random order.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func shuffled() -> [Any]
```

## Return Value

A new array that lists this array’s elements in a random order.

## Discussion

Calling this method is equivalent to calling the shuffled(using:) method and passing the system sharedRandom() random source. To influence the random shuffling or to be able to deterministically reproduce a series of shuffles, create your own GKRandomSource object.

## See Also

### Randomly Shuffling an Array

func shuffled(using: GKRandomSource) -> [Any]

Returns a new array that lists this array’s elements in a random order, using the specified random source.

