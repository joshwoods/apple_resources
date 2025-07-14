

- Foundation
- FileHandle
-  readCompletionNotification 

Type Property

# readCompletionNotification

Posted when the file handle reads the data currently available in a file or at a communications channel.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let readCompletionNotification: NSNotification.Name
```

## Discussion

It makes the data available to observers by putting it in the `userInfo` dictionary. To cause the posting of this notification, you must send either readInBackgroundAndNotify() or readInBackgroundAndNotify(forModes:) to an appropriate `NSFileHandle` object.

The notification object is the `NSFileHandle` object that sent the notification. The `userInfo` dictionary contains the following information:

| Key | Value |
|----|----|
| `NSFileHandleNotificationDataItem` | An `NSData` object containing the available data read from a socket connection. |
| `@"NSFileHandleError"` | An `NSNumber` object containing an integer representing the UNIX-type error which occurred. |

## See Also

### Notifications

static let NSFileHandleConnectionAccepted: NSNotification.Name

Posted when a file handle object establishes a socket connection between two processes, creates a file handle object for one end of the connection, and makes this object available to observers.

static let NSFileHandleDataAvailable: NSNotification.Name

Posted when the file handle determines that data is currently available for reading in a file or at a communications channel.

static let NSFileHandleReadToEndOfFileCompletion: NSNotification.Name

Posted when the file handle reads all data in the file or, in a communications channel, until the other process signals the end of data.

