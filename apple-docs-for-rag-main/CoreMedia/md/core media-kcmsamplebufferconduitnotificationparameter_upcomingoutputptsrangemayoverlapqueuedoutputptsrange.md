

- Core Media
-  kCMSampleBufferConduitNotificationParameter_UpcomingOutputPTSRangeMayOverlapQueuedOutputPTSRange 

Global Variable

# kCMSampleBufferConduitNotificationParameter_UpcomingOutputPTSRangeMayOverlapQueuedOutputPTSRange

Indicates that the presentation timestamps of upcoming output samples may overlap those of samples queued for output (type `CFBoolean`).

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMSampleBufferConduitNotificationParameter_UpcomingOutputPTSRangeMayOverlapQueuedOutputPTSRange: CFString
```

## Discussion

This key is always present in the `userInfo` dictionary for the kCMSampleBufferConduitNotification_UpcomingOutputPTSRangeChanged notification. If its value is kCFBooleanTrue, there is a possibility that upcoming frames may have earlier presentation timestamps than the frames previously provided to the conduit, and the dictionary also contains one or both of the kCMSampleBufferConduitNotificationParameter_MinUpcomingOutputPTS or kCMSampleBufferConduitNotificationParameter_MaxUpcomingOutputPTS keys providing further information. If its value is kCFBooleanFalse, there is no such possibility.

## See Also

### Sample Buffer Conduit Notifications

let kCMSampleBufferConduitNotification_ResetOutput: CFString

Posted on a conduit of sample buffers to request invalidation of pending output data.

let kCMSampleBufferConduitNotification_InhibitOutputUntil: CFString

Posted on a conduit of sample buffers to announce a coming discontinuity.

let kCMSampleBufferConduitNotification_UpcomingOutputPTSRangeChanged: CFString

Posted on a conduit of video sample buffers to report information about the range of upcoming output presentation timestamps.

let kCMSampleBufferConduitNotificationParameter_MinUpcomingOutputPTS: CFString

Specifies the minimum presentation timestamp of upcoming output samples (type `CFDictionary`).

let kCMSampleBufferConduitNotificationParameter_MaxUpcomingOutputPTS: CFString

Specifies the maximum presentation timestamp of upcoming output samples (type `CFDictionary`).

let kCMSampleBufferConduitNotificationParameter_ResumeTag: CFString

Specifies a tag to be attached to the first sample buffer following a discontinuity (type `CFNumber`).

