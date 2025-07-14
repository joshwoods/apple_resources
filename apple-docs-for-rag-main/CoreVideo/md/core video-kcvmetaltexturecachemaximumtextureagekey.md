

- Core Video
-  kCVMetalTextureCacheMaximumTextureAgeKey 

Global Variable

# kCVMetalTextureCacheMaximumTextureAgeKey

The length of time, in seconds, before the cache is automatically evicted.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
let kCVMetalTextureCacheMaximumTextureAgeKey: CFString
```

## Discussion

The default value is `1`. To disable the age-out mechanism completely, set a maximum texture age of `0`. The cache can be manually evicted with CVMetalTextureCacheFlush(_:_:).

## See Also

### Constants

let kCVMetalTextureUsage: CFString

The set of options that define how you can use a texture on the GPU.

