

- Core Media
- CMSampleBuffer
-  setInvalidateHandler(\_:) 

Instance Method

# setInvalidateHandler(\_:)

Sets a closure for the sample buffer to call when it’s invalidated.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setInvalidateHandler(_ body: @escaping (CMSampleBuffer) throws -> Void) throws
```

## Parameters 

`body`  

The invalidation handler.

## Discussion

A sample buffer can only have one invalidation handler.

## See Also

### Invalidating Sample Buffers

var isValid: Bool

A Boolean value that indicates whether the sample buffer is valid.

func invalidate() throws

Invalidates a sample buffer by calling its invalidation handler.

