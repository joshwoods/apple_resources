

- Foundation
- URLSessionStreamTask
-  closeRead() 

Instance Method

# closeRead()

Completes any enqueued reads and writes, and then closes the read side of the underlying socket.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func closeRead()
```

## Discussion

You may continue to write data using the write(_:timeout:completionHandler:) method after calling this method. Any calls to readData(ofMinLength:maxLength:timeout:completionHandler:) after calling this method will result in an error.

## See Also

### Closing read and write sockets

func closeWrite()

Completes any enqueued reads and writes, and then closes the write side of the underlying socket.

