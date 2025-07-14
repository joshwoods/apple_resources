

- Core Media
-  kCMSampleBufferAttachmentKey_TransitionID 

Global Variable

# kCMSampleBufferAttachmentKey_TransitionID

Marks a transition from one source of buffers to another.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMSampleBufferAttachmentKey_TransitionID: CFString
```

## Discussion

For example, during gapless playback of a list of songs, this attachment marks the first buffer from the next song. If this attachment is on a buffer containing no samples, the first following buffer that contains samples is the buffer that contains the first samples from the next song. The value of this attachment is a CFTypeRef. This transition identifier should be unique within a playlist, so each transition in a playlist is uniquely identifiable. A CFNumber counter that increments with each transition is a simple example.

## See Also

### Sample Buffer Keys

let kCMSampleBufferAttachmentKey_DisplayEmptyMediaImmediately: CFString

Tells that the empty marker should be dequeued immediately regardless of its timestamp (type `CFBoolean`, default false).

let kCMSampleBufferAttachmentKey_DrainAfterDecoding: CFString

Indicates whether the sample buffer should be drained after decoding type `CFBoolean`, default false).

let kCMSampleBufferAttachmentKey_DroppedFrameReason: CFString

Indicates the reason the current video frame was dropped (type `CFString`).

let kCMSampleBufferDroppedFrameReason_FrameWasLate: CFString

The frame was dropped because it was late.

let kCMSampleBufferDroppedFrameReason_OutOfBuffers: CFString

The frame was dropped because the module providing frames is out of buffers.

let kCMSampleBufferDroppedFrameReason_Discontinuity: CFString

An unknown number of frames were dropped.

let kCMSampleBufferAttachmentKey_DroppedFrameReasonInfo: CFString

Indicates additional information regarding the dropped video frame (type `CFString`).

let kCMSampleBufferDroppedFrameReasonInfo_CameraModeSwitch: CFString

A discontinuity was caused by a camera mode switch.

let kCMSampleBufferAttachmentKey_EmptyMedia: CFString

Marks an intentionally empty interval in the sequence of samples (type `CFBoolean`, default false).

let kCMSampleBufferAttachmentKey_EndsPreviousSampleDuration: CFString

Indicates that sample buffer’s decode timestamp may be used to define the previous sample buffer’s duration (type `CFBoolean`, default false).

let kCMSampleBufferAttachmentKey_FillDiscontinuitiesWithSilence: CFString

Fill the difference between discontiguous sample buffers with silence (type `CFBoolean`, default false).

let kCMSampleBufferAttachmentKey_ForceKeyFrame: CFString

Indicates that the current or next video sample buffer should be forced to be encoded as a key frame.

let kCMSampleBufferAttachmentKey_GradualDecoderRefresh: CFString

Indicates the decoder refresh count (type `CFNumber`).

let kCMSampleBufferAttachmentKey_PermanentEmptyMedia: CFString

Marks the end of the sequence of samples (type `CFBoolean`, default false).

let kCMSampleBufferAttachmentKey_PostNotificationWhenConsumed: CFString

If present, indicates that decode pipelines should post a notification when consuming the sample buffer(type `CFDictionary`).

