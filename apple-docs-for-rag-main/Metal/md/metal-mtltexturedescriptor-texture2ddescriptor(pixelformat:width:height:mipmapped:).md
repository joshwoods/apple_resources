

- Metal
- MTLTextureDescriptor
-  texture2DDescriptor(pixelFormat:width:height:mipmapped:) 

Type Method

# texture2DDescriptor(pixelFormat:width:height:mipmapped:)

Creates a texture descriptor object for a 2D texture.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class func texture2DDescriptor(
    pixelFormat: MTLPixelFormat,
    width: Int,
    height: Int,
    mipmapped: Bool
) -> MTLTextureDescriptor
```

## Parameters 

`pixelFormat`  

The format describing how every pixel on the texture image is stored. The default value is MTLPixelFormat.rgba8Unorm.

`width`  

The width of the 2D texture image. The value must be greater than or equal to 1.

`height`  

The height of the 2D texture image. The value must be greater than or equal to 1.

`mipmapped`  

A Boolean indicating whether the resulting image should be mipmapped. If true, then the mipmapLevelCount property in the returned descriptor is computed from `width` and `height`. If false, then mipmapLevelCount is `1`.

## Return Value

A pointer to a texture descriptor object for a 2D texture.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Creating Texture Descriptors

class func textureCubeDescriptor(pixelFormat: MTLPixelFormat, size: Int, mipmapped: Bool) -> MTLTextureDescriptor

Creates a texture descriptor object for a cube texture.

class func textureBufferDescriptor(with: MTLPixelFormat, width: Int, resourceOptions: MTLResourceOptions, usage: MTLTextureUsage) -> MTLTextureDescriptor

Creates a texture descriptor object for a texture buffer.

