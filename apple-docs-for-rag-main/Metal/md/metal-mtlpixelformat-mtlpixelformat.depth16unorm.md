

- Metal
- MTLPixelFormat
-  MTLPixelFormat.depth16Unorm 

Case

# MTLPixelFormat.depth16Unorm

A pixel format for a depth-render target that has a 16-bit normalized, unsigned-integer component.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12+tvOS 13.0+visionOS 1.0+

``` source
case depth16Unorm
```

## Discussion

If you need to apply depth bias, choose a different depth format. Setting a depth bias with this format, such as with setDepthBias(_:slopeScale:clamp:), generates incorrect results for apps that run on a device with an Apple A8 or earlier GPU.

## See Also

### Depth and Stencil Pixel Formats

case depth32Float

A pixel format with one 32-bit floating-point component, used for a depth render target.

case stencil8

A pixel format with an 8-bit unsigned integer component, used for a stencil render target.

case depth24Unorm_stencil8

A 32-bit combined depth and stencil pixel format with a 24-bit normalized unsigned integer for depth and an 8-bit unsigned integer for stencil.

case depth32Float_stencil8

A 40-bit combined depth and stencil pixel format with a 32-bit floating-point value for depth and an 8-bit unsigned integer for stencil.

case x32_stencil8

A stencil pixel format used to read the stencil value from a texture with a combined 32-bit depth and 8-bit stencil value.

case x24_stencil8

A stencil pixel format used to read the stencil value from a texture with a combined 24-bit depth and 8-bit stencil value.

