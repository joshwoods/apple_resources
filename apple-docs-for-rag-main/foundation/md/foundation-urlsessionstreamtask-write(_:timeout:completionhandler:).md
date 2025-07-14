

- Foundation
- URLSessionStreamTask
-  write(\_:timeout:completionHandler:) 

Instance Method

# write(\_:timeout:completionHandler:)

Asynchronously writes the specified data to the stream, and calls a handler upon completion.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func write(
    _ data: Data,
    timeout: TimeInterval,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func write(
    _ data: Data,
    timeout: TimeInterval
) async throws
```

## Parameters 

`data`  

The data to be written.

`timeout`  

A timeout for writing bytes. If the write is not completed within the specified interval, the write is canceled and the `completionHandler` is called with an error. Pass `0` to prevent a write from timing out.

`completionHandler`  

The completion handler to call when all bytes are written, or an error occurs. This handler is executed on the delegate queue.

This completion handler takes the following parameter:

`error`  
An error object that indicates why the write failed, or `nil` if the write was successful.

## Discussion

There is no guarantee that the remote side of the stream has received all of the written bytes at the time that `completionHandler` is called, only that all of the data has been written to the kernel.

## See Also

### Reading and writing data

func readData(ofMinLength: Int, maxLength: Int, timeout: TimeInterval, completionHandler: (Data?, Bool, (any Error)?) -> Void)

Asynchronously reads a number of bytes from the stream, and calls a handler upon completion.

