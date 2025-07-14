

- Accelerate
- BNNS
- BNNS.PermuteLayer
-  init(input:output:permutation:filterParameters:) Deprecated

Initializer

# init(input:output:permutation:filterParameters:)

Returns a new permute layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
convenience init?(
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    permutation: [Int],
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

`permutation`  

The array that defines the permutation.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

The number of input dimensions must be equal to number of output dimensions.

