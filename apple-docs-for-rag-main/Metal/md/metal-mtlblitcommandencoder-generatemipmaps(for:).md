

- Metal
- MTLBlitCommandEncoder
-  generateMipmaps(for:) 

Instance Method

# generateMipmaps(for:)

Encodes a command that generates mipmaps for a texture from the base mipmap level up to the highest mipmap level.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func generateMipmaps(for texture: any MTLTexture)
```

**Required**

## Parameters 

`texture`  

A texture instance the command generates mipmaps for that has:

- A mipmapLevelCount property that’s greater than `1`

- A pixelFormat that’s color-renderable and color-filterable

## Mentioned in 

Generating Mipmap Data

## Discussion

The command generates with scaled images for all levels up to the highest mipmap level.

Note

The image filtering that GPU drivers use to generate the mipmaps may vary by the feature families (MTLGPUFamily) it supports.

