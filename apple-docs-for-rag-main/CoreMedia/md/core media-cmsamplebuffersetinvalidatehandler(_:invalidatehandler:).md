

- Core Media
-  CMSampleBufferSetInvalidateHandler(\_:invalidateHandler:) 

Function

# CMSampleBufferSetInvalidateHandler(\_:invalidateHandler:)

Sets the sample buffer’s invalidation handler.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferSetInvalidateHandler(
    _ sbuf: CMSampleBuffer,
    invalidateHandler: @escaping CMSampleBufferInvalidateHandler
) -> OSStatus
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being modified.

`invalidateHandler`  

Block to be called during `CMSampleBufferInvalidate`.

## Discussion

A sample buffer can only have one invalidation callback. The invalidation callback isn’t called during ordinary sample buffer finalization.

## Topics

### Handlers

typealias CMSampleBufferInvalidateHandler

Client callback called by CMSampleBufferInvalidate(_:).

## See Also

### Invalidating Sample Buffers

func CMSampleBufferInvalidate(CMSampleBuffer) -> OSStatus

Invalidates a sample buffer by calling its invalidation callback.

func CMSampleBufferIsValid(CMSampleBuffer) -> Bool

Returns a Boolean value that indicates whether a sample buffer is valid.

func CMSampleBufferSetInvalidateCallback(CMSampleBuffer, callback: CMSampleBufferInvalidateCallback, refcon: UInt64) -> OSStatus

Sets the sample buffer’s invalidation callback.

