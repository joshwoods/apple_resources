

- Core Media
- CMSampleBuffer APIs
-  Sample Attachment Keys 

API Collection

# Sample Attachment Keys

Keys that specify attachments to individual samples in a buffer.

## Overview

You can get and set sample-level attachments in a sample buffer using the CMSampleBufferGetSampleAttachmentsArray(_:createIfNecessary:) function.

## Topics

### Sample Keys

let kCMSampleAttachmentKey_NotSync: CFString

Indicates whether the sample is a sync sample (type `CFBoolean`, default false).

let kCMSampleAttachmentKey_PartialSync: CFString

Indicates whether the sample is a partial sync sample (type `CFBoolean`, default false).

let kCMSampleAttachmentKey_DependsOnOthers: CFString

Indicates whether the sample depends on other samples for decoding (type `CFBoolean`).

let kCMSampleAttachmentKey_IsDependedOnByOthers: CFString

Indicates whether other samples depend on this sample for decoding (type `CFBoolean`).

let kCMSampleAttachmentKey_DisplayImmediately: CFString

Indicates whether the sample should be displayed immediately (type `CFBoolean`, default false).

let kCMSampleAttachmentKey_DoNotDisplay: CFString

Indicates whether the sample should be decoded but not displayed (type `CFBoolean`, default false).

let kCMSampleAttachmentKey_EarlierDisplayTimesAllowed: CFString

Indicates whether later samples may have earlier display times (type `CFBoolean`).

let kCMSampleAttachmentKey_HasRedundantCoding: CFString

Indicates whether the sample has redundant coding (type `CFBoolean`).

let kCMSampleAttachmentKey_PostDecodeProcessingMetadata: CFString

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

let kCMSampleBufferAttachmentKey_ResetDecoderBeforeDecoding: CFString

Indicates whether the sample buffer should be reset before decoding (type `CFBoolean`, default false).

let kCMSampleBufferAttachmentKey_ResumeOutput: CFString

If present, indicates that output should be resumed following a discontinuity `CFBoolean`, default false).

let kCMSampleBufferAttachmentKey_Reverse: CFString

Indicates that the decoded contents of the sample buffer should be reversed (type `CFBoolean`, default false).

let kCMSampleBufferAttachmentKey_SampleReferenceByteOffset: CFString

Indicates the byte offset at which the sample data begins (type `CFNumber`).

let kCMSampleBufferAttachmentKey_SampleReferenceURL: CFString

Indicates the URL where the sample data is (type `CFURL`).

let kCMSampleBufferAttachmentKey_SpeedMultiplier: CFString

The factor by which the sample buffer’s presentation should be accelerated (type `CFNumber`, default 1.0).

let kCMSampleBufferAttachmentKey_StillImageLensStabilizationInfo: CFString

Indicates information about the lens stabilization applied to the current still image buffer.

let kCMSampleBufferLensStabilizationInfo_Active: CFString

The lens stabilization module was active for the duration this buffer.

let kCMSampleBufferLensStabilizationInfo_OutOfRange: CFString

The motion of the device or duration of the capture was outside of what the stabilization mechanism could support.

let kCMSampleBufferLensStabilizationInfo_Unavailable: CFString

The lens stabilization module was unavailable for use.

let kCMSampleBufferLensStabilizationInfo_Off: CFString

The lens stabilization module was not used during this capture.

let kCMSampleBufferAttachmentKey_TransitionID: CFString

Marks a transition from one source of buffers to another.

let kCMSampleBufferAttachmentKey_TrimDurationAtEnd: CFString

The duration that should be removed at the end of the sample buffer, after decoding.

let kCMSampleBufferAttachmentKey_TrimDurationAtStart: CFString

The duration that should be removed at the beginning of the sample buffer, after decoding.

## See Also

### Managing Attachments

func CMSampleBufferGetSampleAttachmentsArray(CMSampleBuffer, createIfNecessary: Bool) -> CFArray?

Retrieves an array of sample attachment dictionaries that represents each sample in a sample buffer.

