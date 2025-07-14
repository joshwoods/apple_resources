

- GameplayKit
- GKMersenneTwisterRandomSource
-  init(seed:) 

Initializer

# init(seed:)

Initializes a random source with the specified seed value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(seed: UInt64)
```

## Parameters 

`seed`  

A seed value for the random number generator.

## Return Value

A new, independent random source.

## Discussion

Any two random sources initialized with the same seed data will generate the same sequence of random numbers. To replicate the behavior of an existing GKMersenneTwisterRandomSource instance, read that instance’s init(seed:) property and then create a new instance by passing the resulting data to the seed initializer.

For a source of high-entropy seed data, see the SecRandomCopyBytes(_:_:_:) function.

## See Also

### Creating a Random Source

convenience init()

Initializes a random source from a nondeterministic seed.

