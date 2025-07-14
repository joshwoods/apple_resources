

- Metal
- MTLPixelFormat
-  MTLPixelFormat.bgra10_xr 

Case

# MTLPixelFormat.bgra10_xr

A 64-bit extended-range pixel format with four fixed-point components of 10-bit blue, 10-bit green, 10-bit red, and 10-bit alpha.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
case bgra10_xr
```

## Discussion

Pixel components are in blue, green, red, and alpha order, from least significant bit to most significant bit (little-endian order). Each component is a 16-bit chunk arranged as follows:

- The 10 most-significant bits (bits 6–15) store the component’s data.

- The 6 least-significant bits (bits 0–5) are padding, and their value is `0`.

The blue, green, and red components are linearly encoded in a transform from `[0,2^10)` to \[`-0.752941, 1.25098]`. The formula used in this linear encoding is `shader_float = (xr10_value - 384) / 510.0f`.

Tip

Each UNorm8-based pixel value has an exact corresponding value in the XR10 pixel range, given by `xr10_value = unorm8_value * 2 + 384`.

The alpha component is always clamped to a `[0.0, 1.0]` range in sampling, rendering, and writing operations, despite supporting values outside this range.

To display wide color values on devices with wide color displays, set this pixel format on the colorPixelFormat property of an MTKView or the pixelFormat property of a CAMetalLayer.

Note

Only devices with a wide color display can display color values outside the `[0.0, 1.0]` range; all other devices clamp color values to the `[0.0, 1.0]` range.

## See Also

### Extended Range and Wide Color Pixel Formats

case bgra10_xr_srgb

A 64-bit extended-range pixel format with sRGB conversion and four fixed-point components of 10-bit blue, 10-bit green, 10-bit red, and 10-bit alpha.

case bgr10_xr

A 32-bit extended-range pixel format with three fixed-point components of 10-bit blue, 10-bit green, and 10-bit red.

case bgr10_xr_srgb

A 32-bit extended-range pixel format with sRGB conversion and three fixed-point components of 10-bit blue, 10-bit green, and 10-bit red.

