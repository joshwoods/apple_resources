

- AVFoundation
- AVSampleBufferDisplayLayer
-  enqueue(\_:) Deprecated

Instance Method

# enqueue(\_:)

Sends a sample buffer for display.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 10.2–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func enqueue(_ sampleBuffer: CMSampleBuffer)
```

Deprecated

Use sampleBufferRenderer's enqueueSampleBuffer: instead

## Parameters 

`sampleBuffer`  

The sample buffer to display.

## Discussion

Apple discourages the use of this symbol in iOS 17, tvOS 17, and macOS 14 and later. Use enqueue(_:) on the sampleBufferRenderer instead.

If `sampleBuffer` has the kCMSampleAttachmentKey_DoNotDisplay attachment set to kCFBooleanTrue, the frame will be decoded but not displayed.

If `sampleBuffer` has the kCMSampleAttachmentKey_DisplayImmediately attachment set to kCFBooleanTrue, the decoded image will be displayed as soon as possible, replacing all previously enqueued images regardless of their timestamps.

Otherwise, the decoded image will be displayed at the `sampleBuffer` output presentation timestamp, as interpreted by the controlTimebase property (or the `mach_absolute_time` timeline if there is no control timebase).

To schedule the removal of previous images at a specific timestamp, enqueue a marker sample buffer containing no samples, with the kCMSampleBufferAttachmentKey_EmptyMedia attachment set to kCFBooleanTrue.

Important

Attachments with the `kCMSampleAttachmentKey_*` prefix must be set via CMSampleBufferGetSampleAttachmentsArray(_:createIfNecessary:) and CFDictionarySetValue(_:_:_:). Attachments with the `kCMSampleBufferAttachmentKey_*` prefix must be set via CMSetAttachment(_:key:value:attachmentMode:).

