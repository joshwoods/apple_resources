

- Metal
- MTLTextureDescriptor
-  textureBufferDescriptor(with:width:resourceOptions:usage:) 

Type Method

# textureBufferDescriptor(with:width:resourceOptions:usage:)

Creates a texture descriptor object for a texture buffer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class func textureBufferDescriptor(
    with pixelFormat: MTLPixelFormat,
    width: Int,
    resourceOptions: MTLResourceOptions = [],
    usage: MTLTextureUsage
) -> MTLTextureDescriptor
```

## Parameters 

`pixelFormat`  

The format describing how every pixel on the texture buffer is stored. The default value is MTLPixelFormat.rgba8Unorm.

`width`  

The width of the texture buffer. The value must be greater than or equal to 1.

`resourceOptions`  

The access options to use for the new texture buffer.

`usage`  

The allowed usage of the new texture buffer.

## Return Value

A pointer to a texture descriptor object for a texture buffer.

## See Also

### Creating Texture Descriptors

class func texture2DDescriptor(pixelFormat: MTLPixelFormat, width: Int, height: Int, mipmapped: Bool) -> MTLTextureDescriptor

Creates a texture descriptor object for a 2D texture.

class func textureCubeDescriptor(pixelFormat: MTLPixelFormat, size: Int, mipmapped: Bool) -> MTLTextureDescriptor

Creates a texture descriptor object for a cube texture.

