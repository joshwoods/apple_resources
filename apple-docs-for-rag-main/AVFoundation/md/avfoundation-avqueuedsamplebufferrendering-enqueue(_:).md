

- AVFoundation
- AVQueuedSampleBufferRendering
-  enqueue(\_:) 

Instance Method

# enqueue(\_:)

Sends a sample buffer to the queue for rendering.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func enqueue(_ sampleBuffer: CMSampleBuffer)
```

**Required**

## Parameters 

`sampleBuffer`  

The sample buffer to be enqueued.

## Discussion

For video data, the sample buffer is processed according to the attachments it contains. If it has a true value for its kCMSampleAttachmentKey_DoNotDisplay attachment, the frame is decoded but not displayed. If it has a `true` value for its kCMSampleAttachmentKey_DisplayImmediately attachment, the frame is displayed as soon as possible, regardless of its presentation timestamp. Otherwise, the frame is displayed according to its presentation timestamp, relative to the timebase.

To schedule the removal of previous images at a specific timestamp, enqueue a marker sample buffer that doesn’t contain any samples, with the kCMSampleBufferAttachmentKey_EmptyMedia attachment set to kCFBooleanTrue.

Important

Attachments with the `kCMSampleAttachmentKey_` prefix must be set using CMSampleBufferGetSampleAttachmentsArray(_:createIfNecessary:) and CFDictionarySetValue(_:_:_:).  Attachments with the `kCMSampleBufferAttachmentKey_` prefix must be set via CMSetAttachment(_:key:value:attachmentMode:).

## See Also

### Requesting Media

var isReadyForMoreMediaData: Bool

A Boolean value that indicates whether the receiver is able to accept more sample buffers.

**Required**

func requestMediaDataWhenReady(on: dispatch_queue_t, using: () -> Void)

Tells the target to invoke a client-supplied block in order to gather sample buffers for playback.

**Required**

func stopRequestingMediaData()

Cancels any current requestMediaDataWhenReady(on:using:) call.

**Required**

