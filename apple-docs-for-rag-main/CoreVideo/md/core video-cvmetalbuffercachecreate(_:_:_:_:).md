

- Core Video
-  CVMetalBufferCacheCreate(\_:\_:\_:\_:) 

Function

# CVMetalBufferCacheCreate(\_:\_:\_:\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func CVMetalBufferCacheCreate(
    _ allocator: CFAllocator?,
    _ cacheAttributes: CFDictionary?,
    _ metalDevice: any MTLDevice,
    _ cacheOut: UnsafeMutablePointer
) -> CVReturn
```

## Discussion

```
@function   CVMetalBufferCacheCreate
@abstract   Creates a new Buffer Cache.
@param      allocator The CFAllocatorRef to use for allocating the cache.  May be NULL.
@param      cacheAttributes A CFDictionaryRef containing the attributes of the cache itself. May be NULL.
@param      metalDevice The Metal device for which the buffer objects will be created.
@param      cacheOut   The newly created buffer cache will be placed here
@result     Returns kCVReturnSuccess on success
```

