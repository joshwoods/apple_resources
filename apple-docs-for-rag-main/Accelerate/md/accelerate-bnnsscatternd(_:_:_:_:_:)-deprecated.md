

- Accelerate
-  BNNSScatterND(\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSScatterND(\_:\_:\_:\_:\_:)

Scatters the slices of a tensor.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSScatterND(
    _ op: BNNSReduceFunction,
    _ input: UnsafePointer,
    _ indices: UnsafePointer,
    _ output: UnsafeMutablePointer,
    _ filter_params: UnsafePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`op`  

The reduction operation that defines how the function combines scattered values with existing output values.

`input`  

A pointer to the input descriptor.

`indices`  

A pointer to the indices descriptor.

`output`  

A pointer to the output descriptor.

`filter_params`  

The filter runtime parameters.

## Discussion

Use BNNSScatterND(_:_:_:_:_:) to scatter slices — that you specify by index — into an output tensor.

The function interprets the indices array as a `k - 1` dimensional set of lookup vectors, therefore, the indices tensor must have `(k - 1) + 1` or `k` dimensions.

If the lookup vectors don’t define a full set of indices, the function treats the undefined indices as a slice.

BNNSScatterND(_:_:_:_:_:) is the inverse of BNNSGatherND(_:_:_:_:). The code samples below are based on the gathered values from the BNNSGatherND(_:_:_:_:) page.

The following code shows that a scalar index scatters a 2D slice:

```
let indices: [Int32] = [1] 
var indicesDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: indices,
    shape: .vector(1))

let gathereredValues: [Float] = [20.0, 21.0, 22.0, 23.0]
var gatheredDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: gathereredValues,
    shape: .matrixFirstMajor(2, 2))

var scatteredDescriptor = BNNSNDArrayDescriptor.allocate(
    repeating: Float(),
    shape: inputDescriptor.shape)

BNNSScatterND(BNNSReduceFunctionNone,
              &gatheredDescriptor,
              &indicesDescriptor,
              &scatteredDescriptor,
              nil)
```

On return, `scatteredDescriptor` contains the following values:

```
[ 0.0,  0.0,
  0.0,  0.0,

 20.0, 21.0,
 22.0, 23.0,

  0.0,  0.0,
  0.0,  0.0 ]
```

The following code shows that a 2D index scatters a 1D slice:

```
let indices: [Int32] = [1, 0] 
var indicesDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: indices,
    shape: .matrixFirstMajor(1, 2))

let gathereredValues: [Float] = [20.0, 21.0]
var gatheredDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: gathereredValues,
    shape: .matrixFirstMajor(1, 2))

var scatteredDescriptor = BNNSNDArrayDescriptor.allocate(
    repeating: Float(),
    shape: inputDescriptor.shape)

BNNSScatterND(BNNSReduceFunctionNone,
              &gatheredDescriptor,
              &indicesDescriptor,
              &scatteredDescriptor,
              nil)  
```

On return, `scatteredDescriptor` contains the following values:

```
[ 0.0,  0.0,
  0.0,  0.0,

 20.0, 21.0,
  0.0,  0.0,

  0.0,  0.0,
  0.0,  0.0 ]
```

The following code shows that a 3D index scatters a single element:

```
let indices: [Int32] = [
    1, 1, 1 
]
var indicesDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: indices,
    shape: .tensor3DFirstMajor(1, 1, 3))

let gathereredValues: [Float] = [23]
var gatheredDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: gathereredValues,
    shape: .matrixFirstMajor(1, 1))

var scatteredDescriptor = BNNSNDArrayDescriptor.allocate(
    repeating: Float(),
    shape: inputDescriptor.shape)

BNNSScatterND(BNNSReduceFunctionNone,
              &gatheredDescriptor,
              &indicesDescriptor,
              &scatteredDescriptor,
              nil)
```

On return, `scatteredDescriptor` contains the following values:

```
[ 0.0,  0.0,
  0.0,  0.0,

  0.0,  0.0,
  0.0, 23.0,

  0.0,  0.0,
  0.0,  0.0 ]
```

If multiple input values update the same output element, the function doesn’t define the order of update operations.

In particular, if you define the reduction as `BNNSReduceFunctionNone` the function doesn’t guarantee any particular value in the result.

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

func BNNSGatherND(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Gathers the slices of a tensor.

Deprecated

func BNNSScatter(Int, BNNSReduceFunction, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Scatters the elements of a tensor along a single axis.

Deprecated

