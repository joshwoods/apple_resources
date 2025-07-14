

- Foundation
- FileHandle
-  waitForDataInBackgroundAndNotify(forModes:) 

Instance Method

# waitForDataInBackgroundAndNotify(forModes:)

Asynchronously checks to see if data is available.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func waitForDataInBackgroundAndNotify(forModes modes: [RunLoop.Mode]?)
```

## Parameters 

`modes`  

The runloop modes in which the data available notification can be posted.

## Discussion

When the data becomes available, this method posts a NSFileHandleDataAvailable notification on the current thread. This method differs from waitForDataInBackgroundAndNotify() in that `modes` specifies the run-loop mode (or modes) in which NSFileHandleDataAvailable can be posted.

You must call this method from a thread that has an active run loop.

## See Also

### Reading Asynchronously with Notifications

func acceptConnectionInBackgroundAndNotify()

Accepts a socket connection (for stream-type sockets only) in the background and creates a file handle for the “near” (client) end of the communications channel.

func acceptConnectionInBackgroundAndNotify(forModes: [RunLoop.Mode]?)

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

