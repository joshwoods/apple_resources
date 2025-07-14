

- Core Video
- CVOpenGLESTextureCache
-  Cache Attributes 

API Collection

# Cache Attributes

Attributes for the texture cache.

## Topics

### Constants

let kCVOpenGLESTextureCacheMaximumTextureAgeKey: CFString

By default, textures will age out after one second. Setting a maximum texture age of zero will disable the age-out mechanism completely. The CVOpenGLESTextureCacheFlush(_:_:) function can be used to force eviction in either case.

Deprecated

