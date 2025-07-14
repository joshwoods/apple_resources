

- Accelerate
-  BNNSGather(\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSGather(\_:\_:\_:\_:\_:)

Gathers the elements of a tensor along a single axis.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSGather(
    _ axis: Int,
    _ input: UnsafePointer,
    _ indices: UnsafePointer,
    _ output: UnsafeMutablePointer,
    _ filter_params: UnsafePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`axis`  

The axis along which the operation gathers the indices.

`input`  

A pointer to the input descriptor.

`indices`  

A pointer to the indices descriptor.

`output`  

A pointer to the output descriptor.

`filter_params`  

The filter runtime parameters.

## Discussion

Use BNNSGather(_:_:_:_:_:) to gather elements — that you specify by index — into an output tensor.

In the simplest case, use BNNSGather(_:_:_:_:_:) to gather elements from a 1D vector with indices defined as a 1D vector. The following code gathers the four elements at indices `[1, 3, 7, 5]`:

```
let values: [Float] = [10, 20, 30, 40, 50, 60, 70, 80]
var inputDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: values,
    shape: .vector(values.count))

let indices: [Int32] = [1, 3, 7, 5]
var indicesDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: indices,
    shape: .vector(indices.count))

var outputDescriptor = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: indicesDescriptor.shape)

let error = BNNSGather(0,
                       &inputDescriptor,
                       &indicesDescriptor,
                       &outputDescriptor,
                       nil)

```

On return, `outputDescriptor` contains the values `[20.0, 40.0, 80.0, 60.0]`.

BNNSGather(_:_:_:_:_:) supports gathering from a tensor with two or more dimensions using indices defined as a 1D vector. In this case, the indices correspond to the values along an entire axis and the input and output shapes must match.

The following code generates a 3 x 4 matrix from the rows of a 3 x 3 matrix:

```
let values: [Float] = [10, 20, 30,
                       40, 50, 60,
                       70, 80, 90]
var inputDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: values,
    shape: .matrixRowMajor(3, 3))

let indices: [Int32] = [0, 1, // Elements `0, 1` from row `0` = `10, 20`
                        2, 0, // Elements `2, 0` from row `1` = `60, 40`
                        1, 1] // Elements `1, 1` from row `2` = `80, 80`
var indicesDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: indices,
    shape: .matrixRowMajor(2, 3))

var outputDescriptor = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: indicesDescriptor.shape)

let error = BNNSGather(1, // axis
                       &inputDescriptor,
                       &indicesDescriptor,
                       &outputDescriptor,
                       nil)
```

On return, `outputDescriptor` contains the following values:

```
 [ 10.0, 20.0,
   60.0, 40.0,
   80.0, 80.0 ]
```

The function returns an error if any of the indices are out of range.

## See Also

### Gather and scatter operations

Calculating the dominant colors in an image

Find the main colors in an image by implementing k-means clustering using the Accelerate framework.

static func gather(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int, filterParameters: BNNSFilterParameters?) throws

Gathers the elements of a tensor along a single axis.

Deprecated

static func gatherND(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Gathers the slices of a tensor.

Deprecated

static func scatter(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int, reductionFunction: BNNS.ReductionFunction, filterParameters: BNNSFilterParameters?) throws

Scatters the elements of a tensor along a single axis.

Deprecated

static func scatterND(input: BNNSNDArrayDescriptor, indices: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, reductionFunction: BNNS.ReductionFunction, filterParameters: BNNSFilterParameters?) throws

Scatters the slices of a tensor.

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

