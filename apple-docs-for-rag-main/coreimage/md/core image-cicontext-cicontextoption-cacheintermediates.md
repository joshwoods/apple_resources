

- Core Image
- CIContext
- CIContextOption
-  cacheIntermediates 

Type Property

# cacheIntermediates

An option for whether the context caches the contents of any intermediate pixel buffers it uses during rendering.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
static let cacheIntermediates: CIContextOption
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value. If this value is `false`, the context empties such buffers during and after renders. The default value is `true`.

