

- Accelerate
-  BNNSShuffle(\_:\_:\_:\_:) Deprecated

Function

# BNNSShuffle(\_:\_:\_:\_:)

Rearranges elements in a tensor according to shuffle type.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSShuffle(
    _ type: BNNSShuffleType,
    _ input: UnsafePointer,
    _ output: UnsafeMutablePointer,
    _ filter_params: UnsafePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`type`  

A constant that specifies the shuffle type.

`input`  

A pointer to the input descriptor.

`output`  

A pointer to the output descriptor.

`filter_params`  

The filter runtime parameters.

## Discussion

Use BNNSShuffle(_:_:_:_:) to rearrange the elements in a tensor between the depth dimension and blocks of 2D spatial data.

Pass a shuffle type of BNNSShuffleTypePixelShuffleNCHW to specify that the function rearranges elements in a tensor of shape `(N,C×r×r,H,W)` to a tensor of shape `(N,C,H×r,W×r)`, where `r` is an upscale factor.

Pass BNNSShuffleTypePixelUnshuffleNCHW to specify that the function elements in a tensor of shape `(N,C,H×r,W×r)` to a tensor of shape `(N,C×r×r,H,W)`, where `r` is a downscale factor.

## See Also

### Errors

enum Error

func BNNSBandPart(Int32, Int32, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Copies the specified subdiagonals and superdiagonals of a matrix, and sets other elements to zero.

Deprecated

struct BNNSShuffleType

Constants that specify a shuffle type.

func BNNSTile(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Generates an output tensor by tiling an input tensor multiple times.

Deprecated

func BNNSTileBackward(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a tile filter backward to generate an input gradient.

Deprecated

