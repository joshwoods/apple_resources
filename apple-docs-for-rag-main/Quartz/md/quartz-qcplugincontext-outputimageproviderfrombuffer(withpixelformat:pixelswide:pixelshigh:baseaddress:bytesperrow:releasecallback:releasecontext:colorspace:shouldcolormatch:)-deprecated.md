

- Quartz
- QCPlugInContext
-  outputImageProviderFromBuffer(withPixelFormat:pixelsWide:pixelsHigh:baseAddress:bytesPerRow:releaseCallback:releaseContext:colorSpace:shouldColorMatch:) Deprecated

Instance Method

# outputImageProviderFromBuffer(withPixelFormat:pixelsWide:pixelsHigh:baseAddress:bytesPerRow:releaseCallback:releaseContext:colorSpace:shouldColorMatch:)

Returns an image provider from a single memory buffer.

macOS 10.4–10.15Deprecated

``` source
func outputImageProviderFromBuffer(
    withPixelFormat format: String!,
    pixelsWide width: Int,
    pixelsHigh height: Int,
    baseAddress: UnsafeRawPointer!,
    bytesPerRow rowBytes: Int,
    releaseCallback callback: QCPlugInBufferReleaseCallback!,
    releaseContext context: UnsafeMutableRawPointer!,
    colorSpace: CGColorSpace!,
    shouldColorMatch colorMatch: Bool
) -> Any!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`format`  

The pixel format of the memory buffer. This must be compatible with the color space.

`width`  

The width, in bytes, of the memory buffer.

`height`  

The height, in bytes, of the memory buffer.

`baseAddress`  

The base address of the memory buffer, which must be multiple of 16.

`rowBytes`  

The number of bytes per row of the memory buffer, which must be multiple of 16.

`callback`  

The release callback. Your callback must use this type definition:

```
typedef void (*QCPlugInBufferReleaseCallback)(const void* address, void* context);
```

If you name your callback function `MyQCPlugInBufferReleaseCallback`, you would declare it like this:

```
void MyQCPlugInBufferReleaseCallback (const void address,
              void * context);
```

Quartz Composer invokes your callback when the memory buffer is no longer needed. The callback can be called from any thread at any time

`context`  

The context to pass to the release callback.

`colorSpace`  

The color space of the memory buffer. This must be compatible with the pixel format.

`colorMatch`  

A Boolean that specifies whether Quartz Composer should color match the image. Pass false if the image is a mask or gradient or should not be color matched for some other reason. Otherwise, pass true.

## Return Value

An image provider.

## Discussion

You must not modify the image until the release callback is invoked.

## See Also

### Getting an Image Provider

func outputImageProviderFromTexture(withPixelFormat: String!, pixelsWide: Int, pixelsHigh: Int, name: GLuint, flipped: Bool, releaseCallback: QCPlugInTextureReleaseCallback!, releaseContext: UnsafeMutableRawPointer!, colorSpace: CGColorSpace!, shouldColorMatch: Bool) -> Any!

Returns an image provider from an OpenGL texture.

**Required**

Deprecated

