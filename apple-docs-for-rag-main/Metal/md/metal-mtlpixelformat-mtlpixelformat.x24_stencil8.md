

- Metal
- MTLPixelFormat
-  MTLPixelFormat.x24_stencil8 

Case

# MTLPixelFormat.x24_stencil8

A stencil pixel format used to read the stencil value from a texture with a combined 24-bit depth and 8-bit stencil value.

Mac Catalyst 13.0+macOS 10.12+

``` source
case x24_stencil8
```

## Discussion

You can’t directly read the stencil value of a texture with the MTLPixelFormat.depth24Unorm_stencil8 format. To read stencil values from a texture with the MTLPixelFormat.depth24Unorm_stencil8 format, create a texture view of that texture using the MTLPixelFormat.x24_stencil8 format, and sample the texture view instead.

## See Also

### Depth and Stencil Pixel Formats

case depth16Unorm

A pixel format for a depth-render target that has a 16-bit normalized, unsigned-integer component.

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

