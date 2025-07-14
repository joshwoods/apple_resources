

- GameplayKit
- GKARC4RandomSource
-  init(seed:) 

Initializer

# init(seed:)

Initializes a random source with the specified seed data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(seed: Data)
```

## Parameters 

`seed`  

A data object containing seed values for the random number generator.

## Return Value

A new, independent random source.

## Discussion

Any two random sources initialized with the same seed data will generate the same sequence of random numbers. To replicate the behavior of an existing GKARC4RandomSource instance, read that instance’s seed property and then create a new instance by passing the resulting data to the init(seed:) initializer.

For a source of high-entropy seed data, see the SecRandomCopyBytes(_:_:_:) function.

## See Also

### Creating a Random Source

convenience init()

Initializes a random source from a nondeterministic seed.

