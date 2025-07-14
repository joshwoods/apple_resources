

- Foundation
- FileHandle
-  acceptConnectionInBackgroundAndNotify(forModes:) 

Instance Method

# acceptConnectionInBackgroundAndNotify(forModes:)

Accepts a socket connection (for stream-type sockets only) in the background and creates a file handle for the “near” (client) end of the communications channel.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func acceptConnectionInBackgroundAndNotify(forModes modes: [RunLoop.Mode]?)
```

## Parameters 

`modes`  

The runloop modes in which the connection accepted notification can be posted.

## Discussion

See acceptConnectionInBackgroundAndNotify() for details of how this method operates. This method differs from acceptConnectionInBackgroundAndNotify() in that `modes` specifies the run-loop mode (or modes) in which NSFileHandleConnectionAccepted can be posted.

You must call this method from a thread that has an active run loop.

## See Also

### Related Documentation

func enqueue(Notification, postingStyle: NotificationQueue.PostingStyle, coalesceMask: NotificationQueue.NotificationCoalescing, forModes: [RunLoop.Mode]?)

Adds a notification to the notification queue with a specified posting style, criteria for coalescing, and run loop mode.

### Reading Asynchronously with Notifications

func acceptConnectionInBackgroundAndNotify()

Accepts a socket connection (for stream-type sockets only) in the background and creates a file handle for the “near” (client) end of the communications channel.

func readInBackgroundAndNotify()

Reads from the file or communications channel in the background and posts a notification when finished.

func readInBackgroundAndNotify(forModes: [RunLoop.Mode]?)

Reads from the file or communications channel in the background and posts a notification when finished.

func readToEndOfFileInBackgroundAndNotify()

Reads to the end of file from the file or communications channel in the background and posts a notification when finished.

func readToEndOfFileInBackgroundAndNotify(forModes: [RunLoop.Mode]?)

Reads to the end of file from the file or communications channel in the background and posts a notification when finished.

func waitForDataInBackgroundAndNotify()

Asynchronously checks to see if data is available.

func waitForDataInBackgroundAndNotify(forModes: [RunLoop.Mode]?)

Asynchronously checks to see if data is available.

