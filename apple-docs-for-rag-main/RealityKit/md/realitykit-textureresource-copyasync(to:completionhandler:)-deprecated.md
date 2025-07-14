

- RealityKit
- TextureResource
-  copyAsync(to:completionHandler:) Deprecated

Instance Method

# copyAsync(to:completionHandler:)

Asynchronously copies texture data to another texture.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor @preconcurrency
func copyAsync(
    to texture: any MTLTexture,
    completionHandler: @escaping @MainActor ((any Error)?) -> Void
)
```

## Parameters 

`texture`  

The target texture for copying the data. It needs to have the same width and height as TextureResource, and shaderWrite usage.

`completionHandler`  

The system calls this closure after it finishes copying the data, with a `nil` error if it succeeds.

## Discussion

This function is asynchronous. It returns immediately and runs in the background, calling `completionHandler` when it finishes or errors. This method copies all available mipmap sizes to `texture`.

It’s recommended that you provide a value for semantic when creating this resource. Specifying a semantic enables RealityKit to select an appropriate pixel format for the target texture.

## See Also

### Copying the texture

func copy(to: any MTLTexture) async throws

Asynchronously copies texture data to another texture.

func copy(to: any MTLTexture) throws

Copies texture data to another texture.

