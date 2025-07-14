

- Core Media
-  CMSampleBufferSetInvalidateCallback(\_:callback:refcon:) 

Function

# CMSampleBufferSetInvalidateCallback(\_:callback:refcon:)

Sets the sample buffer’s invalidation callback.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferSetInvalidateCallback(
    _ sbuf: CMSampleBuffer,
    callback invalidateCallback: CMSampleBufferInvalidateCallback,
    refcon invalidateRefCon: UInt64
) -> OSStatus
```

## Parameters 

`sbuf`  

The sample buffer being modified.

`invalidateCallback`  

Reference to a function to be called during `CMSampleBufferInvalidate`.

`invalidateRefCon`  

Reference constant to be passed to `invalidateCallback`.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

A sample buffer can only have one invalidation callback. The invalidation callback *isn’t* called during ordinary sample buffer finalization.

## Topics

### Callbacks

typealias CMSampleBufferInvalidateCallback

Client callback called by CMSampleBufferInvalidate(_:).

## See Also

### Invalidating Sample Buffers

func CMSampleBufferSetInvalidateHandler(CMSampleBuffer, invalidateHandler: CMSampleBufferInvalidateHandler) -> OSStatus

Sets the sample buffer’s invalidation handler.

func CMSampleBufferInvalidate(CMSampleBuffer) -> OSStatus

Invalidates a sample buffer by calling its invalidation callback.

func CMSampleBufferIsValid(CMSampleBuffer) -> Bool

Returns a Boolean value that indicates whether a sample buffer is valid.

