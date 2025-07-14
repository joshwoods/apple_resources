

- Quartz
- QCPlugInContext
-  outputImageProviderFromTexture(withPixelFormat:pixelsWide:pixelsHigh:name:flipped:releaseCallback:releaseContext:colorSpace:shouldColorMatch:) Deprecated

Instance Method

# outputImageProviderFromTexture(withPixelFormat:pixelsWide:pixelsHigh:name:flipped:releaseCallback:releaseContext:colorSpace:shouldColorMatch:)

Returns an image provider from an OpenGL texture.

macOS 10.5–10.14Deprecated

``` source
func outputImageProviderFromTexture(
    withPixelFormat format: String!,
    pixelsWide width: Int,
    pixelsHigh height: Int,
    name: GLuint,
    flipped: Bool,
    releaseCallback callback: QCPlugInTextureReleaseCallback!,
    releaseContext context: UnsafeMutableRawPointer!,
    colorSpace: CGColorSpace!,
    shouldColorMatch colorMatch: Bool
) -> Any!
```

**Required**

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`format`  

The pixel format of the texture. This must be compatible with the color space.

`width`  

The width, in bytes, of the texture.

`height`  

The height, in bytes, of the texture.

`name`  

An OpenGL texture of type `GL_TEXTURE_RECTANGLE_EXT` that is valid on the Quartz Composer OpenGL context. Your application must make sure that the texture exists for the life cycle of the image provider.

`flipped`  

true to have Quartz Composer flip the contents of the texture vertically.

`callback`  

The release callback. Your callback must use this type definition:

```
typedef void (*QCPlugInTextureReleaseCallback)(CGLContextObj cgl_ctx, GLuint name, void* context);
```

If you name your callback function `MyQCPlugInTextureReleaseCallback`, you would declare it like this:

```
void MyQCPlugInTextureReleaseCallback (CGLContextObj cgl_ctx,
              GLuint name,
              void* context);
```

Quartz Composer invokes your callback when the memory buffer is no longer needed. The callback can be called from any thread at any time

`context`  

The context to pass to the release callback.

`colorSpace`  

The color space of the texture. This must be compatible with the pixel format.

`colorMatch`  

A Boolean that specifies whether Quartz Composer should color match the texture. Pass false if the texture is a mask or gradient or should not be color matched for some other reason. Otherwise, pass true.

## Return Value

An image provider.

## Discussion

You must not modify the texture until the release callback is invoked.

## See Also

### Getting an Image Provider

func outputImageProviderFromBuffer(withPixelFormat: String!, pixelsWide: Int, pixelsHigh: Int, baseAddress: UnsafeRawPointer!, bytesPerRow: Int, releaseCallback: QCPlugInBufferReleaseCallback!, releaseContext: UnsafeMutableRawPointer!, colorSpace: CGColorSpace!, shouldColorMatch: Bool) -> Any!

Returns an image provider from a single memory buffer.

**Required**

Deprecated

