

- Core Media
-  kCMSampleBufferConduitNotificationParameter_ResumeTag 

Global Variable

# kCMSampleBufferConduitNotificationParameter_ResumeTag

Specifies a tag to be attached to the first sample buffer following a discontinuity (type `CFNumber`).

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMSampleBufferConduitNotificationParameter_ResumeTag: CFString
```

## Discussion

A conduit of sample buffers posts the kCMSampleBufferConduitNotification_InhibitOutputUntil notification when a discontinuity in decoding occurs. The value for this key will be attached to the first sample buffer following the discontinuity using the kCMSampleBufferAttachmentKey_ResumeOutput attachment, indicating that clients should resume output.

## See Also

### Sample Buffer Conduit Notifications

let kCMSampleBufferConduitNotification_ResetOutput: CFString

Posted on a conduit of sample buffers to request invalidation of pending output data.

let kCMSampleBufferConduitNotification_InhibitOutputUntil: CFString

Posted on a conduit of sample buffers to announce a coming discontinuity.

let kCMSampleBufferConduitNotification_UpcomingOutputPTSRangeChanged: CFString

Posted on a conduit of video sample buffers to report information about the range of upcoming output presentation timestamps.

let kCMSampleBufferConduitNotificationParameter_UpcomingOutputPTSRangeMayOverlapQueuedOutputPTSRange: CFString

Indicates that the presentation timestamps of upcoming output samples may overlap those of samples queued for output (type `CFBoolean`).

let kCMSampleBufferConduitNotificationParameter_MinUpcomingOutputPTS: CFString

Specifies the minimum presentation timestamp of upcoming output samples (type `CFDictionary`).

let kCMSampleBufferConduitNotificationParameter_MaxUpcomingOutputPTS: CFString

Specifies the maximum presentation timestamp of upcoming output samples (type `CFDictionary`).

