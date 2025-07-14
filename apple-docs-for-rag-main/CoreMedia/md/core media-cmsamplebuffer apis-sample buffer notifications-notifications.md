

- Core Media
- CMSampleBuffer APIs
-  Sample Buffer Notifications 

API Collection

# Sample Buffer Notifications

Notifications the system posts when processing sample buffer objects.

## Topics

### Sample Buffer Notifications

let kCMSampleBufferNotification_DataBecameReady: CFString

Posted on a sample buffer by the CMSampleBufferSetDataReady(_:) function when the buffer becomes ready.

let kCMSampleBufferNotification_DataFailed: CFString

let kCMSampleBufferNotificationParameter_OSStatus: CFString

let kCMSampleBufferConsumerNotification_BufferConsumed: CFString

Optionally posted when a sample buffer is consumed.

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

let kCMSampleBufferConduitNotificationParameter_ResumeTag: CFString

Specifies a tag to be attached to the first sample buffer following a discontinuity (type `CFNumber`).

