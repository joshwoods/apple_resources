

- Core Media
- CMSampleBuffer
-  invalidate() 

Instance Method

# invalidate()

Invalidates a sample buffer by calling its invalidation handler.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func invalidate() throws
```

## Discussion

You can’t use a sample buffer after invalidating it; all of its accessors throw errors.

Important

Don’t invalidate a sample buffer that another process is accessing concurrently.

## See Also

### Invalidating Sample Buffers

var isValid: Bool

A Boolean value that indicates whether the sample buffer is valid.

func setInvalidateHandler((CMSampleBuffer) throws -> Void) throws

Sets a closure for the sample buffer to call when it’s invalidated.

