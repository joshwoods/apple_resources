

- Accelerate
- BNNS
- BNNS.RandomGenerator
-  init(method:seed:filterParameters:) 

Initializer

# init(method:seed:filterParameters:)

Returns a new random number generator.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
init?(
    method: BNNS.RandomGeneratorMethod,
    seed: UInt64? = nil,
    filterParameters: BNNSFilterParameters? = nil
)
```

## Parameters 

`method`  

The random number generation method.

`seed`  

An optional unsigned integer value the function uses to initialize the random number generator.

`filterParameters`  

The runtime filter parameters.

## See Also

### Creating a Random Number Generator

enum RandomGeneratorMethod

Constants that describe random number generation methods.

