

- Accelerate
-  BNNSTileBackward(\_:\_:\_:) Deprecated

Function

# BNNSTileBackward(\_:\_:\_:)

Applies a tile filter backward to generate an input gradient.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSTileBackward(
    _ in_delta: UnsafeMutablePointer,
    _ out_delta: UnsafePointer,
    _ filter_params: UnsafePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`in_delta`  

A pointer to the input delta descriptor.

`out_delta`  

A pointer to the output delta descriptor.

`filter_params`  

The filter runtime parameters.

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

func BNNSTile(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Generates an output tensor by tiling an input tensor multiple times.

Deprecated

