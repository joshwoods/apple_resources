

- Accelerate
-  BNNSTile(\_:\_:\_:) Deprecated

Function

# BNNSTile(\_:\_:\_:)

Generates an output tensor by tiling an input tensor multiple times.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSTile(
    _ input: UnsafePointer,
    _ output: UnsafeMutablePointer,
    _ filter_params: UnsafePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`input`  

A pointer to the input descriptor.

`output`  

A pointer to the output descriptor.

`filter_params`  

The filter runtime parameters.

## Discussion

Use BNNSTile(_:_:_:) to tile generate a tensor by repeating tiled copies of the input tensor. The dimensions of the output tensor must be an integer multiple of the corresponding dimension of the input tensor.

For example, the following code tiles a 2 x 3 matrix three times along the first dimension and twice along the second dimension:

```
let values: [Float] = [1.0, 2.0, 3.0,
                       4.0, 5.0, 6.0]

var inputDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: values,
    shape: .matrixRowMajor(2, 3))

var outputDescriptor = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: .matrixRowMajor(6, 6))

BNNSTile(&inputDescriptor, &outputDescriptor, nil)

inputDescriptor.deallocate()
outputDescriptor.deallocate()
```

On return, `outputDescriptor` contains the following values:

```
[ 1.0, 2.0, 3.0,  1.0, 2.0, 3.0,
  4.0, 5.0, 6.0,  4.0, 5.0, 6.0,

  1.0, 2.0, 3.0,  1.0, 2.0, 3.0,
  4.0, 5.0, 6.0,  4.0, 5.0, 6.0,

  1.0, 2.0, 3.0,  1.0, 2.0, 3.0,
  4.0, 5.0, 6.0,  4.0, 5.0, 6.0 ]
```

## See Also

### Errors

enum Error

func BNNSBandPart(Int32, Int32, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Copies the specified subdiagonals and superdiagonals of a matrix, and sets other elements to zero.

Deprecated

func BNNSShuffle(BNNSShuffleType, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Rearranges elements in a tensor according to shuffle type.

Deprecated

struct BNNSShuffleType

Constants that specify a shuffle type.

func BNNSTileBackward(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a tile filter backward to generate an input gradient.

Deprecated

