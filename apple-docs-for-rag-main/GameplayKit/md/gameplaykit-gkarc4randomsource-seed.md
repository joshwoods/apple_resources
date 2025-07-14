

- GameplayKit
- GKARC4RandomSource
-  seed 

Instance Property

# seed

The seed data that determines the random source’s behavior.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var seed: Data { get set }
```

## Discussion

Any two random sources initialized with the same seed data will generate the same sequence of random numbers. To replicate the behavior of an existing GKARC4RandomSource instance, read this property and then create a new instance by passing the resulting data to the init(seed:) initializer.

For a source of high-entropy seed data, see the SecRandomCopyBytes(_:_:_:) function.

