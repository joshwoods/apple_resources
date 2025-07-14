

- Core Video
-  kCVOpenGLESTextureCacheMaximumTextureAgeKey Deprecated

Global Variable

# kCVOpenGLESTextureCacheMaximumTextureAgeKey

By default, textures will age out after one second. Setting a maximum texture age of zero will disable the age-out mechanism completely. The CVOpenGLESTextureCacheFlush(_:_:) function can be used to force eviction in either case.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
let kCVOpenGLESTextureCacheMaximumTextureAgeKey: CFString
```

Deprecated

OpenGL/OpenGLES is no longer supported. Use Metal APIs instead. (Define COREVIDEO_SILENCE_GL_DEPRECATION to silence these warnings)

