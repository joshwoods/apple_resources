

- Metal
- MTLPixelFormat
-  MTLPixelFormat.bgrg422 

Case

# MTLPixelFormat.bgrg422

A pixel format where the red and green components are subsampled horizontally.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case bgrg422
```

## Discussion

Two pixels are stored in 32 bits, with shared red and blue values, and unique green values. The component arrangement is the same as it is in UYVY, 2vuy, and k2vuy pixel formats, except there is no implicit format conversion from a YUV to RGB color space. Only 2D non-mipmapped textures can be created with this pixel format, and the width must be a multiple of 2. Neither MTLTextureType.type2DArray nor MTLTextureType.typeCube textures are supported. This format is a compressed format with a block size of 2x1 in a 32-bit block.

## See Also

### YUV Pixel Formats

case gbgr422

A pixel format where the red and green components are subsampled horizontally.

