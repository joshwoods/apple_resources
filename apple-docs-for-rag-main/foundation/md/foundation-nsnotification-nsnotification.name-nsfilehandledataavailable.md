

- Foundation
- NSNotification
- NSNotification.Name
-  NSFileHandleDataAvailable 

Type Property

# NSFileHandleDataAvailable

Posted when the file handle determines that data is currently available for reading in a file or at a communications channel.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let NSFileHandleDataAvailable: NSNotification.Name
```

## Discussion

The observers can then issue the appropriate messages to begin reading the data. To cause the posting of this notification, you must send either waitForDataInBackgroundAndNotify() or waitForDataInBackgroundAndNotify(forModes:) to an appropriate `NSFileHandle` object.

The notification object is the `NSFileHandle` object that sent the notification. This notification doesn’t contain a `userInfo` dictionary.

## See Also

### Notifications

static let NSFileHandleConnectionAccepted: NSNotification.Name

Posted when a file handle object establishes a socket connection between two processes, creates a file handle object for one end of the connection, and makes this object available to observers.

class let readCompletionNotification: NSNotification.Name

Posted when the file handle reads the data currently available in a file or at a communications channel.

static let NSFileHandleReadToEndOfFileCompletion: NSNotification.Name

Posted when the file handle reads all data in the file or, in a communications channel, until the other process signals the end of data.

