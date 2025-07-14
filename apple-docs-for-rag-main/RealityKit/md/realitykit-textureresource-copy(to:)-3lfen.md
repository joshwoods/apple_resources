

- RealityKit
- TextureResource
-  copy(to:) 

Instance Method

# copy(to:)

Asynchronously copies texture data to another texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func copy(to texture: any MTLTexture) async throws
```

## Parameters 

`texture`  

The target texture for copying the data. It needs to have the same width and height as TextureResource, and shaderWrite usage.

## Discussion

This method copies all available mipmap sizes to `texture`.

It’s recommended that you provide a value for semantic when creating this resource. Specifying a semantic enables RealityKit to select an appropriate pixel format for the target texture.

## See Also

### Copying the texture

func copy(to: any MTLTexture) throws

Copies texture data to another texture.

func copyAsync(to: any MTLTexture, completionHandler: ((any Error)?) -> Void)

Asynchronously copies texture data to another texture.

Deprecated

