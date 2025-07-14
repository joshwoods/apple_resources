

- Accelerate
- BNNS
-  gather(input:indices:output:axis:filterParameters:) Deprecated

Type Method

# gather(input:indices:output:axis:filterParameters:)

Gathers the elements of a tensor along a single axis.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func gather(
    input: BNNSNDArrayDescriptor,
    indices: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    axis: Int,
    filterParameters: BNNSFilterParameters? = nil
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`input`  

The input descriptor.

`indices`  

The indices descriptor.

`output`  

The output descriptor.

`axis`  

The axis along which the operation gathers the indices.

`filterParameters`  

The filter runtime parameters.

## See Also

### Related Documentation

func BNNSGather(Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Gathers the elements of a tensor along a single axis.

Deprecated

### Gather and scatter operations

Calculating the dominant colors in an image

Find the main colors in an image by implementing k-means clustering using the Accelerate framework.

static func gatherND(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Gathers the slices of a tensor.

Deprecated

static func scatter(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int, reductionFunction: BNNS.ReductionFunction, filterParameters: BNNSFilterParameters?) throws

Scatters the elements of a tensor along a single axis.

Deprecated

static func scatterND(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, reductionFunction: BNNS.ReductionFunction, filterParameters: BNNSFilterParameters?) throws

Scatters the slices of a tensor.

Deprecated

func BNNSGather(Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Gathers the elements of a tensor along a single axis.

Deprecated

func BNNSGatherND(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Gathers the slices of a tensor.

Deprecated

func BNNSScatter(Int, BNNSReduceFunction, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Scatters the elements of a tensor along a single axis.

Deprecated

func BNNSScatterND(BNNSReduceFunction, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Scatters the slices of a tensor.

Deprecated

