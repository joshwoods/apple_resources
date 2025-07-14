

- Foundation
-  URLSessionDataDelegate 

Protocol

# URLSessionDataDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to data and upload tasks.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol URLSessionDataDelegate : URLSessionTaskDelegate
```

## Mentioned in 

Fetching website data into memory

Accessing cached data

## Overview

Your session delegate should also implement the methods in the URLSessionTaskDelegate protocol to handle task-level events that are common to all task types, and methods in the URLSessionDelegate protocol to handle session-level events.

Note

A URLSession object need not have a delegate. If no delegate is assigned, when you create tasks in that session, you must provide a completion handler block to obtain the data.

Completion handler blocks are primarily intended as an alternative to using a custom delegate. If you create a task using a method that takes a completion handler block, the delegate methods for response and data delivery are not called.

## Topics

### Handling task life cycle changes

func urlSession(URLSession, dataTask: URLSessionDataTask, didReceive: URLResponse, completionHandler: (URLSession.ResponseDisposition) -> Void)

Tells the delegate that the data task received the initial reply (headers) from the server.

enum ResponseDisposition

Constants indicating how a data or upload session should proceed after receiving the initial headers.

func urlSession(URLSession, dataTask: URLSessionDataTask, didBecome: URLSessionDownloadTask)

Tells the delegate that the data task was changed to a download task.

func urlSession(URLSession, dataTask: URLSessionDataTask, didBecome: URLSessionStreamTask)

Tells the delegate that the data task was changed to a stream task.

### Receiving data

func urlSession(URLSession, dataTask: URLSessionDataTask, didReceive: Data)

Tells the delegate that the data task has received some of the expected data.

### Handling caching

func urlSession(URLSession, dataTask: URLSessionDataTask, willCacheResponse: CachedURLResponse, completionHandler: (CachedURLResponse?) -> Void)

Asks the delegate whether the data (or upload) task should store the response in the cache.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable
- URLSessionDelegate
- URLSessionTaskDelegate

## See Also

### Adding data tasks to a session

func dataTask(with: URL) -> URLSessionDataTask

Creates a task that retrieves the contents of the specified URL.

func dataTask(with: URL, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionDataTask

Creates a task that retrieves the contents of the specified URL, then calls a handler upon completion.

func dataTask(with: URLRequest) -> URLSessionDataTask

Creates a task that retrieves the contents of a URL based on the specified URL request object.

func dataTask(with: URLRequest, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionDataTask

Creates a task that retrieves the contents of a URL based on the specified URL request object, and calls a handler upon completion.

class URLSessionDataTask

A URL session task that returns downloaded data directly to the app in memory.

