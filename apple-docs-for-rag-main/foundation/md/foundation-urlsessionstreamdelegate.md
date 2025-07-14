

- Foundation
-  URLSessionStreamDelegate 

Protocol

# URLSessionStreamDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to stream tasks.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol URLSessionStreamDelegate : URLSessionTaskDelegate
```

## Overview

In addition to these methods, be sure to implement the methods in the URLSessionTaskDelegate and URLSessionDelegate protocols to handle events common to all task types and session-level events, respectively.

Note

A URLSession object need not have a delegate. If no delegate is assigned, a system-provided delegate is used, and you must provide a completion callback to obtain the data.

## Topics

### Handling rerouting

func urlSession(URLSession, betterRouteDiscoveredFor: URLSessionStreamTask)

Tells the delegate that a better route to the host has been detected for the stream.

### Completing stream capture

func urlSession(URLSession, streamTask: URLSessionStreamTask, didBecome: InputStream, outputStream: OutputStream)

Tells the delegate that the stream task has been completed as a result of the stream task calling the captureStreams() method.

### Handling closing events

func urlSession(URLSession, readClosedFor: URLSessionStreamTask)

Tells the delegate that the read side of the underlying socket has been closed.

func urlSession(URLSession, writeClosedFor: URLSessionStreamTask)

Tells the delegate that the write side of the underlying socket has been closed.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable
- URLSessionDelegate
- URLSessionTaskDelegate

## See Also

### Adding stream tasks to a session

func streamTask(withHostName: String, port: Int) -> URLSessionStreamTask

Creates a task that establishes a bidirectional TCP/IP connection to a specified hostname and port.

func streamTask(with: NetService) -> URLSessionStreamTask

Creates a task that establishes a bidirectional TCP/IP connection using a specified network service.

Deprecated

class URLSessionStreamTask

A URL session task that is stream-based.

