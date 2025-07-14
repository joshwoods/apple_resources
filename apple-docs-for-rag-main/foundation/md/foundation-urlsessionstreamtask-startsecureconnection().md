

- Foundation
- URLSessionStreamTask
-  startSecureConnection() 

Instance Method

# startSecureConnection()

Completes any enqueued reads and writes, and establishes a secure connection.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func startSecureConnection()
```

## Discussion

Authentication callbacks are sent to the session’s delegate using the urlSession(_:task:didReceive:completionHandler:) method.

## See Also

### Starting and stopping secure connections

func stopSecureConnection()

Completes any enqueued reads and writes, and closes the secure connection.

Deprecated

