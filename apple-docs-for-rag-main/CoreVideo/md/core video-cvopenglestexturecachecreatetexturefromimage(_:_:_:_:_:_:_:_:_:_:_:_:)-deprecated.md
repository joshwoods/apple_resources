

- Core Video
-  CVOpenGLESTextureCacheCreateTextureFromImage(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# CVOpenGLESTextureCacheCreateTextureFromImage(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Creates a CVOpenGLESTexture object from an existing CVImageBuffer.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
func CVOpenGLESTextureCacheCreateTextureFromImage(
    _ allocator: CFAllocator?,
    _ textureCache: CVOpenGLESTextureCache,
    _ sourceImage: CVImageBuffer,
    _ textureAttributes: CFDictionary?,
    _ target: GLenum,
    _ internalFormat: GLint,
    _ width: GLsizei,
    _ height: GLsizei,
    _ format: GLenum,
    _ type: GLenum,
    _ planeIndex: Int,
    _ textureOut: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`allocator`  

The CFAllocator to use for allocating the texture object. This parameter can be `NULL`.

`textureCache`  

The texture cache object that will manage the texture.

`sourceImage`  

The CVImageBuffer that you want to create a texture from.

`textureAttributes`  

A CFDictionary containing the attributes to be used for creating the CVOpenGLESTexture objects. This parameter can be `NULL`.

`target`  

The target texture. `GL_TEXTURE_2D` and `GL_RENDERBUFFER` are the only targets currently supported.

`internalFormat`  

The number of color components in the texture. Examples are `GL_RGBA`, `GL_LUMINANCE`, `GL_RGBA8_OES`, `GL_RED`, and `GL_RG`.

`width`  

The width of the texture image.

`height`  

The height of the texture image.

`format`  

The format of the pixel data. Examples are `GL_RGBA` and `GL_LUMINANCE`.

`type`  

The data type of the pixel data. One example is `GL_UNSIGNED_BYTE`.

`planeIndex`  

The plane of the CVImageBuffer to map bind. Ignored for non-planar CVImageBuffers.

`textureOut`  

A pointer to a CVOpenGLESTexture where the newly created texture object will be placed.

## Return Value

Upon successful creation of the texture, this function returns kCVReturnSuccess.

## Discussion

This function either creates a new or returns a cached CVOpenGLESTexture texture object mapped to the CVImageBuffer and associated parameters. This operation creates a live binding between the image buffer and the underlying texture object. The EAGLContext associated with the cache may be modified to create, delete, or bind textures. When used as a source texture or `GL_COLOR_ATTACHMENT`, the image buffer must be unlocked before rendering. The source or render buffer texture should not be re-used until the rendering has completed. This can be guaranteed by calling `glFlush()`.

Some example mappings can be seen in the following code snippet.

```
//Mapping a BGRA buffer as a source texture:
CVOpenGLESTextureCacheCreateTextureFromImage(kCFAllocatorDefault, textureCache, pixelBuffer, NULL, GL_TEXTURE_2D, GL_RGBA, width, height, GL_RGBA, GL_UNSIGNED_BYTE, 0, &outTexture);
//Mapping a BGRA buffer as a renderbuffer:
CVOpenGLESTextureCacheCreateTextureFromImage(kCFAllocatorDefault, textureCache, pixelBuffer, NULL, GL_RENDERBUFFER, GL_RGBA8_OES, width, height, GL_RGBA, GL_UNSIGNED_BYTE, 0, &outTexture);
//Mapping the luma plane of a 420v buffer as a source texture:
CVOpenGLESTextureCacheCreateTextureFromImage(kCFAllocatorDefault, textureCache, pixelBuffer, NULL, GL_TEXTURE_2D, GL_LUMINANCE, width, height, GL_LUMINANCE, GL_UNSIGNED_BYTE, 0, &outTexture);
//Mapping the chroma plane of a 420v buffer as a source texture:
CVOpenGLESTextureCacheCreateTextureFromImage(kCFAllocatorDefault, textureCache, pixelBuffer, NULL, GL_TEXTURE_2D, GL_LUMINANCE_ALPHA, width/2, height/2, GL_LUMINANCE_ALPHA, GL_UNSIGNED_BYTE, 1, &outTexture);
//Mapping a yuvs buffer as a source texture (note: yuvs/f and 2vuy are unpacked and resampled -- not colorspace converted)
CVOpenGLESTextureCacheCreateTextureFromImage(kCFAllocatorDefault, textureCache, pixelBuffer, NULL, GL_TEXTURE_2D, GL_RGB_422_APPLE, width, height, GL_RGB_422_APPLE, GL_UNSIGNED_SHORT_8_8_APPLE, 1, &outTexture);
```

## See Also

### Functions

func CVOpenGLESTextureCacheCreate(CFAllocator?, CFDictionary?, CVEAGLContext, CFDictionary?, UnsafeMutablePointer&lt;CVOpenGLESTextureCache?>) -> CVReturn

Creates a new Core Video texture cache.

Deprecated

func CVOpenGLESTextureCacheFlush(CVOpenGLESTextureCache, CVOptionFlags)

Performs internal housekeeping/recycling operations on a texture cache.

Deprecated

func CVOpenGLESTextureCacheGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a Core Video texture cache.

Deprecated

