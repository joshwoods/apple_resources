

- Core Media
-  kCMSampleBufferConsumerNotification_BufferConsumed 

Global Variable

# kCMSampleBufferConsumerNotification_BufferConsumed

Optionally posted when a sample buffer is consumed.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMSampleBufferConsumerNotification_BufferConsumed: CFString
```

## Discussion

If a sample buffer has a value for the kCMSampleBufferAttachmentKey_PostNotificationWhenConsumed attachment, an object that consumes the sample buffer should post this notification with itself as the notifying object and the attachment value as the `userInfo` dictionary.

## See Also

### Sample Buffer Notifications

let kCMSampleBufferNotification_DataBecameReady: CFString

Posted on a sample buffer by the CMSampleBufferSetDataReady(_:) function when the buffer becomes ready.

let kCMSampleBufferNotification_DataFailed: CFString

let kCMSampleBufferNotificationParameter_OSStatus: CFString

