

- Core Media
-  kCMSampleBufferConduitNotification_InhibitOutputUntil 

Global Variable

# kCMSampleBufferConduitNotification_InhibitOutputUntil

Posted on a conduit of sample buffers to announce a coming discontinuity.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMSampleBufferConduitNotification_InhibitOutputUntil: CFString
```

## Discussion

A conduit of sample buffers (for example, a buffer queue; see CMBufferQueue APIs) posts this notification when a discontinuity in decoding occurs. The `userInfo` dictionary for this notification contains the kCMSampleBufferConduitNotificationParameter_ResumeTag key, whose value specifies a tag that indicates when output should resume.

The first sample buffer following the discontinuity should have a kCMSampleBufferAttachmentKey_ResumeOutput attachment whose value is the same number as the resume tag announced in this notification. The consumer should discard output data until it receives this sample buffer. If multiple notifications of this type are received, the last one indicates the resume tag.

## See Also

### Sample Buffer Conduit Notifications

let kCMSampleBufferConduitNotification_ResetOutput: CFString

Posted on a conduit of sample buffers to request invalidation of pending output data.

let kCMSampleBufferConduitNotification_UpcomingOutputPTSRangeChanged: CFString

Posted on a conduit of video sample buffers to report information about the range of upcoming output presentation timestamps.

let kCMSampleBufferConduitNotificationParameter_UpcomingOutputPTSRangeMayOverlapQueuedOutputPTSRange: CFString

Indicates that the presentation timestamps of upcoming output samples may overlap those of samples queued for output (type `CFBoolean`).

let kCMSampleBufferConduitNotificationParameter_MinUpcomingOutputPTS: CFString

Specifies the minimum presentation timestamp of upcoming output samples (type `CFDictionary`).

let kCMSampleBufferConduitNotificationParameter_MaxUpcomingOutputPTS: CFString

Specifies the maximum presentation timestamp of upcoming output samples (type `CFDictionary`).

let kCMSampleBufferConduitNotificationParameter_ResumeTag: CFString

Specifies a tag to be attached to the first sample buffer following a discontinuity (type `CFNumber`).

