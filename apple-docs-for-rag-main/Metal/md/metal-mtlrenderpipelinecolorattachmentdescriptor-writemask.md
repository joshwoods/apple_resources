

- Metal
- MTLRenderPipelineColorAttachmentDescriptor
-  writeMask 

Instance Property

# writeMask

A bitmask that restricts which color channels are written into the texture.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var writeMask: MTLColorWriteMask { get set }
```

## Discussion

The default value of `writeMask` is all ones, all, which allows all color channels to be blended. The `MTLColorWriteMask` values `MTLColorWriteMaskRed`, `MTLColorWriteMaskGreen`, `MTLColorWriteMaskBlue`, and `MTLColorWriteMaskAlpha` limit blending to one color channel, and these values can be bitwise combined. `MTLColorWriteMaskNone` does not allow any color channels to be blended.

## See Also

### Specifying Render Pipeline State

var pixelFormat: MTLPixelFormat

The pixel format of the color attachment’s texture.

