

- Metal
- MTLPixelFormat
-  MTLPixelFormat.depth24Unorm_stencil8 

Case

# MTLPixelFormat.depth24Unorm_stencil8

A 32-bit combined depth and stencil pixel format with a 24-bit normalized unsigned integer for depth and an 8-bit unsigned integer for stencil.

Mac Catalyst 13.0+macOS 10.11+

``` source
case depth24Unorm_stencil8
```

## Discussion

To blit either the depth or stencil information to a Metal buffer, call the copy(from:sourceSlice:sourceLevel:sourceOrigin:sourceSize:to:destinationOffset:destinationBytesPerRow:destinationBytesPerImage:options:) method, specifying the blit options for which part you want to copy. You must provide space for 4 bytes per pixel in your destination buffer. When Metal copies the data, it sets the bottom 3 bytes of each pixel to the depth data and sets the top byte to arbitrary data. Ignore any data stored in the top byte of each pixel.

## See Also

### Depth and Stencil Pixel Formats

case depth16Unorm

A pixel format for a depth-render target that has a 16-bit normalized, unsigned-integer component.

case depth32Float

A pixel format with one 32-bit floating-point component, used for a depth render target.

case stencil8

A pixel format with an 8-bit unsigned integer component, used for a stencil render target.

case depth32Float_stencil8

A 40-bit combined depth and stencil pixel format with a 32-bit floating-point value for depth and an 8-bit unsigned integer for stencil.

case x32_stencil8

A stencil pixel format used to read the stencil value from a texture with a combined 32-bit depth and 8-bit stencil value.

case x24_stencil8

A stencil pixel format used to read the stencil value from a texture with a combined 24-bit depth and 8-bit stencil value.

