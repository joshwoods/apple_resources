

- Accelerate
- BNNS
-  computeNormBackward(input:output:axes:outputGradient:generatingInputGradient:) Deprecated

Type Method

# computeNormBackward(input:output:axes:outputGradient:generatingInputGradient:)

Backpropogates gradients for the compute norm function.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
static func computeNormBackward(
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    axes: [Int]? = nil,
    outputGradient: BNNSNDArrayDescriptor,
    generatingInputGradient inputGradient: BNNSNDArrayDescriptor
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`axes`  

The indices of the axes over which the function computes the norm. Set to `nil` to specify that the function computes the norm over the entire tensor.

`outputGradient`  

The descriptor of the output delta.

`inputGradient`  

The descriptor of the input delta.

## See Also

### Compute norm functions

static func computeNorm(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?) throws

Computes the Euclidean norm and writes the result to the output tensor.

Deprecated

func BNNSComputeNorm(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSNormType, UInt32) -> Int32

Computes the specified norm over an entire tensor or the specified axes.

Deprecated

func BNNSComputeNormBackward(UnsafeRawPointer, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafeRawPointer, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSNormType, UInt32) -> Int32

Backpropogates gradients for the compute norm function.

Deprecated

struct BNNSNormType

Constants that describe norm types.

