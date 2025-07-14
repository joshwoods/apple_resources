

- Core Media
-  CMSampleBufferInvalidate(\_:) 

Function

# CMSampleBufferInvalidate(\_:)

Invalidates a sample buffer by calling its invalidation callback.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferInvalidate(_ sbuf: CMSampleBuffer) -> OSStatus
```

## Parameters 

`sbuf`  

The sample buffer to invalidate.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

An invalid sample buffer can’t be used — all accessors will return kCMSampleBufferError_Invalidated.

Important

You shouldn’t invalidate a sample buffer that another module may be accessing concurrently.

## See Also

### Invalidating Sample Buffers

func CMSampleBufferSetInvalidateHandler(CMSampleBuffer, invalidateHandler: CMSampleBufferInvalidateHandler) -> OSStatus

Sets the sample buffer’s invalidation handler.

func CMSampleBufferIsValid(CMSampleBuffer) -> Bool

Returns a Boolean value that indicates whether a sample buffer is valid.

func CMSampleBufferSetInvalidateCallback(CMSampleBuffer, callback: CMSampleBufferInvalidateCallback, refcon: UInt64) -> OSStatus

Sets the sample buffer’s invalidation callback.

