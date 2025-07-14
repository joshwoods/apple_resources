

- Core Media
- CMSampleBuffer
-  isValid 

Instance Property

# isValid

A Boolean value that indicates whether the sample buffer is valid.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isValid: Bool { get }
```

## See Also

### Invalidating Sample Buffers

func setInvalidateHandler((CMSampleBuffer) throws -> Void) throws

Sets a closure for the sample buffer to call when it’s invalidated.

func invalidate() throws

Invalidates a sample buffer by calling its invalidation handler.

