

- Metal Performance Shaders Graph
- MPSGraph
-  randomPhiloxStateTensor(withCounterLow:counterHigh:key:name:) 

Instance Method

# randomPhiloxStateTensor(withCounterLow:counterHigh:key:name:)

Creates a tensor representing state using the Philox algorithm with given counter and key values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func randomPhiloxStateTensor(
    withCounterLow counterLow: Int,
    counterHigh: Int,
    key: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`counterLow`  

The value to initilaize lower 64 bits of counter to. Philox utilizes a 128 bit counter

`counterHigh`  

The value to initilaize upper 64 bits of counter to. Philox utilizes a 128 bit counter

`key`  

The value to initialize the key to in Philox algorithm.

`name`  

Name for the operation

## Return Value

An MPSGraphTensor representing a random state, to be passed as an input to a random op.

## Discussion

See randomPhiloxStateTensorWithSeed.

