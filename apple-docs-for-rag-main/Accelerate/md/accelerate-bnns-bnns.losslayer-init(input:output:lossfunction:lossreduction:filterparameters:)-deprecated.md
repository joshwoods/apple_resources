

- Accelerate
- BNNS
- BNNS.LossLayer
-  init(input:output:lossFunction:lossReduction:filterParameters:) Deprecated

Initializer

# init(input:output:lossFunction:lossReduction:filterParameters:)

Returns a new loss layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
convenience init?(
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    lossFunction: BNNS.LossFunction,
    lossReduction: BNNS.LossReduction,
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`lossFunction`  

The function that’s used to compute the loss.

`lossReduction`  

The function that’s used to reduce the computed loss.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

The input data type and output data type must be `float`. The output size must be `1`, unless the reduction is BNNS.LossReduction.none.

