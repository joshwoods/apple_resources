

- Foundation
- URLSessionStreamTask
-  closeWrite() 

Instance Method

# closeWrite()

Completes any enqueued reads and writes, and then closes the write side of the underlying socket.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func closeWrite()
```

## Discussion

You may continue to read data using the readData(ofMinLength:maxLength:timeout:completionHandler:) method after calling this method. Any calls to write(_:timeout:completionHandler:) after calling this method will result in an error.

Because the server may continue to write bytes to the client, it is recommended that you continue reading until the stream reaches end-of-file (EOF).

## See Also

### Closing read and write sockets

func closeRead()

Completes any enqueued reads and writes, and then closes the read side of the underlying socket.

