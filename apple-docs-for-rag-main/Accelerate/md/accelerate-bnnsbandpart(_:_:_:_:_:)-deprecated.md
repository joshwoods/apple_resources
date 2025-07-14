

- Accelerate
-  BNNSBandPart(\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSBandPart(\_:\_:\_:\_:\_:)

Copies the specified subdiagonals and superdiagonals of a matrix, and sets other elements to zero.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSBandPart(
    _ num_lower: Int32,
    _ num_upper: Int32,
    _ input: UnsafePointer,
    _ output: UnsafeMutablePointer,
    _ filter_params: UnsafePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`num_lower`  

The number of subdiagonals that the function copies. Set to a negative value to copy the entire lower triangle.

`num_upper`  

The number of superdiagonals that the function copies. Set to a negative value to copy the entire upper triangle.

`input`  

A pointer to the input descriptor.

`output`  

A pointer to the output descriptor.

`filter_params`  

The filter runtime parameters.

## Discussion

Use BNNSBandPart(_:_:_:_:_:) to copy a tensor’s main diagonal and zero or more upper and lower bands. You can specify that the function returns either the entire upper or lower triangle by passing a negative value to the corresponding `num_*` parameter.

For example, given the following 8x8 matrix:

```
let matrixValues: [Float] = [ 11, 12, 13, 14, 15, 16, 17, 18,
                              21, 22, 23, 24, 25, 26, 27, 28,
                              31, 32, 33, 34, 35, 36, 37, 38,
                              41, 42, 43, 44, 45, 46, 47, 48,
                              51, 52, 53, 54, 55, 56, 57, 58,
                              61, 62, 63, 64, 65, 66, 67, 68,
                              71, 72, 73, 74, 75, 76, 77, 78,
                              81, 82, 83, 84, 85, 86, 87, 88 ]

var inputDescriptor = BNNSNDArrayDescriptor.allocate(
     initializingFrom: matrixValues,
     shape: .matrixRowMajor(8, 8))
```

The following code selects the upper triangle and sets other elements to zero:

```
var outputDescriptor = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: inputDescriptor.shape)

BNNSBandPart(0,  // num_lower
             -1, // num_upper
             &inputDescriptor,
             &outputDescriptor, nil)

printMatrix(outputDescriptor)
```

On return, `outputDescriptor` contains the following values:

```
11.0, 12.0, 13.0, 14.0, 15.0, 16.0, 17.0, 18.0
 0.0, 22.0, 23.0, 24.0, 25.0, 26.0, 27.0, 28.0
 0.0,  0.0, 33.0, 34.0, 35.0, 36.0, 37.0, 38.0
 0.0,  0.0,  0.0, 44.0, 45.0, 46.0, 47.0, 48.0
 0.0,  0.0,  0.0,  0.0, 55.0, 56.0, 57.0, 58.0
 0.0,  0.0,  0.0,  0.0,  0.0, 66.0, 67.0, 68.0
 0.0,  0.0,  0.0,  0.0,  0.0,  0.0, 77.0, 78.0
 0.0,  0.0,  0.0,  0.0,  0.0,  0.0,  0.0, 88.0
```

The following code selects the 4 subdiagonals, 1 superdiagonal, and sets other elements to zero:

```
var outputDescriptor = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: inputDescriptor.shape)

BNNSBandPart(4, // num_lower
             1, // num_upper
             &inputDescriptor,
             &outputDescriptor, nil)

printMatrix(outputDescriptor)
```

On return, `outputDescriptor` contains the following values:

```
11.0, 12.0,  0.0,  0.0,  0.0,  0.0,  0.0,  0.0
21.0, 22.0, 23.0,  0.0,  0.0,  0.0,  0.0,  0.0
31.0, 32.0, 33.0, 34.0,  0.0,  0.0,  0.0,  0.0
41.0, 42.0, 43.0, 44.0, 45.0,  0.0,  0.0,  0.0
51.0, 52.0, 53.0, 54.0, 55.0, 56.0,  0.0,  0.0
 0.0, 62.0, 63.0, 64.0, 65.0, 66.0, 67.0,  0.0
 0.0,  0.0, 73.0, 74.0, 75.0, 76.0, 77.0, 78.0
 0.0,  0.0,  0.0, 84.0, 85.0, 86.0, 87.0, 88.0
```

## See Also

### Errors

enum Error

func BNNSShuffle(BNNSShuffleType, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Rearranges elements in a tensor according to shuffle type.

Deprecated

struct BNNSShuffleType

Constants that specify a shuffle type.

func BNNSTile(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Generates an output tensor by tiling an input tensor multiple times.

Deprecated

func BNNSTileBackward(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a tile filter backward to generate an input gradient.

Deprecated

