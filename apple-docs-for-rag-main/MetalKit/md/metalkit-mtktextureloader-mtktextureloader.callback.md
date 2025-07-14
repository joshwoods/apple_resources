

- MetalKit
- MTKTextureLoader
-  MTKTextureLoader.Callback 

Type Alias

# MTKTextureLoader.Callback

The signature for the block executed after an asynchronous loading operation for a single texture has completed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
typealias Callback = ((any MTLTexture)?, (any Error)?) -> Void
```

## Discussion

The block parameters are defined as follows:

texture  
A MTLTexture object, or `nil` if an error occurred.

error  
If the operation was successful, this value is `nil`; otherwise, this parameter holds an NSError object that describes the problem that occurred.

## See Also

### Completing a Texture Loading Operation

typealias ArrayCallback

The signature for the block executed after an asynchronous loading operation for multiple textures has completed.

