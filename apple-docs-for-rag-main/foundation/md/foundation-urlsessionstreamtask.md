

- Foundation
-  URLSessionStreamTask 

Class

# URLSessionStreamTask

A URL session task that is stream-based.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class URLSessionStreamTask
```

## Overview

URLSessionStreamTask is a concrete subclass of URLSessionTask. Many of the methods in the URLSessionStreamTask class are documented in URLSessionTask.

The URLSessionStreamTask class provides an interface a TCP/IP connection created via URLSession. Tasks may be created from an URLSession using the streamTask(withHostName:port:) and streamTask(with:) methods. They may also be created as a result of an URLSessionDataTask being upgraded via the HTTP `Upgrade:` response header and appropriate use of the httpShouldUsePipelining option of URLSessionConfiguration.

Note

See RFC 2817 and RFC 6455 for information about the `Upgrade:` header.

A URLSessionStreamTask object performs asynchronous reads and writes, which are enqueued and executed serially, calling a handler upon completion being on the session delegate queue. If the task is canceled, all enqueued reads and writes will call their completion handlers with an appropriate error.

When working with APIs that accept Stream objects, you can create InputStream and OutputStream objects from an URLSessionStreamTask object by calling the captureStreams() method.

Note

watchOS supports URLSessionStreamTask for specific use cases. For more details, see TN3135: Low-level networking on watchOS.

## Topics

### Reading and writing data

func readData(ofMinLength: Int, maxLength: Int, timeout: TimeInterval, completionHandler: (Data?, Bool, (any Error)?) -> Void)

Asynchronously reads a number of bytes from the stream, and calls a handler upon completion.

func write(Data, timeout: TimeInterval, completionHandler: ((any Error)?) -> Void)

Asynchronously writes the specified data to the stream, and calls a handler upon completion.

### Capturing streams

func captureStreams()

Completes any already enqueued reads and writes, and then invokes the urlSession(_:streamTask:didBecome:outputStream:) delegate message.

### Closing read and write sockets

func closeRead()

Completes any enqueued reads and writes, and then closes the read side of the underlying socket.

func closeWrite()

Completes any enqueued reads and writes, and then closes the write side of the underlying socket.

### Starting and stopping secure connections

func startSecureConnection()

Completes any enqueued reads and writes, and establishes a secure connection.

func stopSecureConnection()

Completes any enqueued reads and writes, and closes the secure connection.

Deprecated

### Initializers

init()Deprecated

### Type Methods

class func new() -> SelfDeprecated

## Relationships

### Inherits From

- URLSessionTask

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- ProgressReporting
- Sendable

## See Also

### Adding stream tasks to a session

func streamTask(withHostName: String, port: Int) -> URLSessionStreamTask

Creates a task that establishes a bidirectional TCP/IP connection to a specified hostname and port.

func streamTask(with: NetService) -> URLSessionStreamTask

Creates a task that establishes a bidirectional TCP/IP connection using a specified network service.

Deprecated

protocol URLSessionStreamDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to stream tasks.

