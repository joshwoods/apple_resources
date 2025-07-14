

- Core Media
-  CMSampleBufferIsValid(\_:) 

Function

# CMSampleBufferIsValid(\_:)

Returns a Boolean value that indicates whether a sample buffer is valid.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferIsValid(_ sbuf: CMSampleBuffer) -> Bool
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being interrogated.

## Return Value

A Boolean indicating whether the sample buffer is still valid.

## Discussion

Returns false if `sbuf` is `NULL` or `CMSampleBufferInvalidate` was called, true otherwise. Doesn’t perform any kind of exhaustive validation of the sample buffer.

## See Also

### Invalidating Sample Buffers

func CMSampleBufferSetInvalidateHandler(CMSampleBuffer, invalidateHandler: CMSampleBufferInvalidateHandler) -> OSStatus

Sets the sample buffer’s invalidation handler.

func CMSampleBufferInvalidate(CMSampleBuffer) -> OSStatus

Invalidates a sample buffer by calling its invalidation callback.

func CMSampleBufferSetInvalidateCallback(CMSampleBuffer, callback: CMSampleBufferInvalidateCallback, refcon: UInt64) -> OSStatus

Sets the sample buffer’s invalidation callback.

