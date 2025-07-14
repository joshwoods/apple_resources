

- Metal
- MTLTextureDescriptor
-  textureCubeDescriptor(pixelFormat:size:mipmapped:) 

Type Method

# textureCubeDescriptor(pixelFormat:size:mipmapped:)

Creates a texture descriptor object for a cube texture.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class func textureCubeDescriptor(
    pixelFormat: MTLPixelFormat,
    size: Int,
    mipmapped: Bool
) -> MTLTextureDescriptor
```

## Parameters 

`pixelFormat`  

The format describing how every pixel on the texture image is stored. The default value is MTLPixelFormat.rgba8Unorm.

`size`  

The width and height of each slice of the cube texture. The value must be greater than or equal to 1.

`mipmapped`  

A Boolean indicating whether the resulting image should be mipmapped. If true, then the mipmapLevelCount property in the returned descriptor is computed from `width` and `height`. If false, then mipmapLevelCount is `1`.

## Return Value

A pointer to a texture descriptor object for a cube texture.

## Discussion

For a cube texture, the property values describe one slice, which is any one of its six sides. Each slice is a square.

## See Also

### Creating Texture Descriptors

class func texture2DDescriptor(pixelFormat: MTLPixelFormat, width: Int, height: Int, mipmapped: Bool) -> MTLTextureDescriptor

Creates a texture descriptor object for a 2D texture.

class func textureBufferDescriptor(with: MTLPixelFormat, width: Int, resourceOptions: MTLResourceOptions, usage: MTLTextureUsage) -> MTLTextureDescriptor

Creates a texture descriptor object for a texture buffer.

