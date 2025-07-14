

- Accelerate
-  BNNSGatherND(\_:\_:\_:\_:) Deprecated

Function

# BNNSGatherND(\_:\_:\_:\_:)

Gathers the slices of a tensor.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSGatherND(
    _ input: UnsafePointer,
    _ indices: UnsafePointer,
    _ output: UnsafeMutablePointer,
    _ filter_params: UnsafePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`input`  

A pointer to the input descriptor.

`indices`  

A pointer to the indices descriptor.

`output`  

A pointer to the output descriptor.

`filter_params`  

The filter runtime parameters.

## Discussion

Use BNNSGatherND(_:_:_:_:) to gather slices — that you specify by index — into an output tensor.

The function interprets the indices array as a `k - 1` dimensional set of lookup vectors, therefore, the indices tensor must have `(k - 1) + 1` or `k` dimensions.

If the lookup vectors don’t define a full set of indices, the function treats the undefined indices as a slice.

For example, given the following input values:

```
let values: [Float] = [10, 11,
                       12, 13,

                       20, 21,
                       22, 23,

                       30, 31,
                       32, 33]

var inputDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: values,
    shape: .tensor3DFirstMajor(3, 2, 2))
```

The following code shows that a scalar index gathers a 2D slice:

```
let indices: [Int32] = [1] // Elements `20, 21, 22, 23` from slice `1`
var indicesDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: indices,
    shape: .vector(1))

var outputDescriptor = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: .matrixFirstMajor(2, 2))

let error = BNNSGatherND(&inputDescriptor,
                         &indicesDescriptor,
                         &outputDescriptor,
                         nil)

// `outputDescriptor` contains `[20.0, 21.0, 22.0, 23.0]`   
```

The following code shows that a 2D index gathers a 1D slice:

```
let indices: [Int32] = [1, 0] // Elements `20, 21` from row `0` of slice `1`
var indicesDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: indices,
    shape: .matrixFirstMajor(1, 2))

var outputDescriptor = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: .matrixFirstMajor(1, 2))

let error = BNNSGatherND(&inputDescriptor,
                         &indicesDescriptor,
                         &outputDescriptor,
                         nil)

// `outputDescriptor` contains `[20.0, 21.0]`
```

The following code shows that a 3D index gathers a single element:

```
let indices: [Int32] = [1, 1, 1] // Element `23` (index `1`) from row `1` of slice `1`
var indicesDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: indices,
    shape: .tensor3DFirstMajor(1, 1, 3))

var outputDescriptor = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: .matrixFirstMajor(1, 1))

let error = BNNSGatherND(&inputDescriptor,
                         &indicesDescriptor,
                         &outputDescriptor,
                         nil)

// `outputDescriptor` contains `[23.0]`  
```

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

func BNNSGather(Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Gathers the elements of a tensor along a single axis.

Deprecated

func BNNSScatter(Int, BNNSReduceFunction, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Scatters the elements of a tensor along a single axis.

Deprecated

func BNNSScatterND(BNNSReduceFunction, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Scatters the slices of a tensor.

Deprecated

