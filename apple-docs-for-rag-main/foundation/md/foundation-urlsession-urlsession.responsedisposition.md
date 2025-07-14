

- Foundation
- URLSession
-  URLSession.ResponseDisposition 

Enumeration

# URLSession.ResponseDisposition

Constants indicating how a data or upload session should proceed after receiving the initial headers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum ResponseDisposition
```

## Overview

When a data or upload task first receives a response, it calls the urlSession(_:dataTask:didReceive:completionHandler:) method of URLSessionDataDelegate. Implement this method to inspect the received URLResponse and then call the provided completion handler. The first parameter to the completion handler is of this type, a disposition that tells the task how to proceed.

## Topics

### Task dispositions

case cancel

Cancel the load.

case allow

Allow the load operation to continue.

case becomeDownload

Convert the response for this request to use a URLSessionDownloadTask.

case becomeStream

Convert the response for this request to use a URLSessionStreamTask.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling task life cycle changes

func urlSession(URLSession, dataTask: URLSessionDataTask, didReceive: URLResponse, completionHandler: (URLSession.ResponseDisposition) -> Void)

Tells the delegate that the data task received the initial reply (headers) from the server.

func urlSession(URLSession, dataTask: URLSessionDataTask, didBecome: URLSessionDownloadTask)

Tells the delegate that the data task was changed to a download task.

func urlSession(URLSession, dataTask: URLSessionDataTask, didBecome: URLSessionStreamTask)

Tells the delegate that the data task was changed to a stream task.

