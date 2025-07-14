

- Core Video
- CVOpenGLTextureCache
-  Cache Attributes 

API Collection

# Cache Attributes

Dictionary keys and values for use with the cacheAttributes parameter of CVOpenGLTextureCacheCreate(_:_:_:_:_:_:)

## Overview

In some cases, a texture cache can do higher quality chroma upsampling on GPUs that support `ARB_fragment_program`. By default, it will be enabled automatically if the texture cache determines that the GPU has the needed support and the image size is something reasonable for the GPU being used. The default behavior can be overridden using the values defined below.

Note

Setting the chroma sampling mode to `kCVOpenGLTextureCacheChromaSamplingModeHighQuality` is only a request. GPUs that don’t support `ARB_fragment_program` will still resort back to the native hardware support for YCbCr textures.

## Topics

### Key

let kCVOpenGLTextureCacheChromaSamplingModeKey: CFString

The key used to define the cache’s requested chroma sampling mode.

Deprecated

### Values

let kCVOpenGLTextureCacheChromaSamplingModeAutomatic: CFString

The default mode if not otherwise specified.

Deprecated

let kCVOpenGLTextureCacheChromaSamplingModeHighestQuality: CFString

Forces the highest quality regardless of performance impact.

Deprecated

let kCVOpenGLTextureCacheChromaSamplingModeBestPerformance: CFString

Set the chroma sample mode to use the most performant way possible.

Deprecated

