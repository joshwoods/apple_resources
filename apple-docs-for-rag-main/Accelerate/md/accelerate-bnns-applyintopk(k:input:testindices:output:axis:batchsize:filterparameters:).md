

- Accelerate
- BNNS
-  applyInTopK(k:input:testIndices:output:axis:batchSize:filterParameters:) 

Type Method

# applyInTopK(k:input:testIndices:output:axis:batchSize:filterParameters:)

Applies an in-top-k filter directly to an input.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func applyInTopK(
    k: Int,
    input: BNNSNDArrayDescriptor,
    testIndices: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    axis: Int,
    batchSize: Int,
    filterParameters: BNNSFilterParameters? = nil
) throws
```

## Parameters 

`k`  

The number of entries the operation finds.

`input`  

The descriptor of the input.

`testIndices`  

The descriptor of the test indices.

`output`  

The descriptor of the output.

`axis`  

The axis along which the operation finds top-k entries.

`batchSize`  

The number of input-output pairs to process.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

The input data type must be `float`, the test indices data type must be `int32`, and the output data type must be `BNNSDataTypeBoolean`.

## See Also

### Related Documentation

func BNNSDirectApplyInTopK(Int, Int, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies an in-top-k filter directly to an input.

### Top-k layers

static func applyTopK(k: Int, input: BNNSNDArrayDescriptor, bestValues: BNNSNDArrayDescriptor, bestIndices: BNNSNDArrayDescriptor, axis: Int, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies a top-k filter directly to an input.

