

- Accelerate
- BNNS
-  computeNorm(input:output:axes:) Deprecated

Type Method

# computeNorm(input:output:axes:)

Computes the Euclidean norm and writes the result to the output tensor.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+watchOS 8.0+visionOS

``` source
static func computeNorm(
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    axes: [Int]? = nil
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

## Discussion

Use this function to compute the norm of either an entire tensor or an axis or axes of a tensor.

For example, the following code defines a 3D tensor:

```
let inputValues: [Float] = [1, 2, 3,
                            4, 5, 6,

                            10, 20, 30,
                            40, 50, 60,

                            100, 200, 300,
                            400, 500, 600,

                            1000, 2000, 3000,
                            4000, 5000, 6000]

let input = BNNSNDArrayDescriptor.allocate(
    initializingFrom: inputValues,
    shape: .imageCHW(3, 2, 4))
```

Define the `axes` parameter as either `[0, 1, 2]` or `nil` to specify that the operation computes the norm of the entire tensor. In this case, the norm is a scalar value, and the destination’s data layout must be a BNNS.DataLayout.vector with a size of `1`.

```
let output = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: .vector(1))

try? BNNS.computeNorm(input: input,
                     output: output,
                     axes: [0, 1, 2])

// Prints `[9587.45]`.
print(output.makeArray(of: Float.self)!)
```

On return, the output descriptor contains a single value that is the square root of the sum of squares of each element in the tensor:

Specify an `axes` of `[2]` to compute the norms along the second axis. In this case, the destination must be a matrix with a size that matches the zeroth and first dimensions of the source tensor:

```
let output = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: .matrixColumnMajor(3, 2))

try? BNNS.computeNorm(input: input,
                     output: output,
                     axes: [2])

// Prints
//      [1005.0378, 2010.075, 3015.113,
//       4020.1511, 5025.189, 6030.227]
print(output.makeArray(of: Float.self)!)
```

On return, the output descriptor contains six values that are the norms of the slices along the second axis of the input tensor:

To compute the norm along more that one dimension, define the destination tensor with a size of the dimensions you’re not calculating over. For example, the following code defines an `axes` with a value of `[0, 2]` to compute the norm of dimensions zero and two:

```
let output = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: .vector(2))

try? BNNS.computeNorm(input: input,
                     output: output,
                     axes: [0, 2])

// Prints `[3760.507, 8819.171]`
print(output.makeArray(of: Float.self)!)
```

On return, the output descriptor contains two values that are the norms of the top and bottom slices of the input tensor:

## See Also

### Compute norm functions

static func computeNormBackward(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor) throws

Backpropogates gradients for the compute norm function.

Deprecated

func BNNSComputeNorm(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSNormType, UInt32) -> Int32

Computes the specified norm over an entire tensor or the specified axes.

Deprecated

func BNNSComputeNormBackward(UnsafeRawPointer, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafeRawPointer, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSNormType, UInt32) -> Int32

Backpropogates gradients for the compute norm function.

Deprecated

struct BNNSNormType

Constants that describe norm types.

