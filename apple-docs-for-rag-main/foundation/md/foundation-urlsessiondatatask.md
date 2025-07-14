

- Foundation
-  URLSessionDataTask 

Class

# URLSessionDataTask

A URL session task that returns downloaded data directly to the app in memory.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class URLSessionDataTask
```

## Mentioned in 

Fetching website data into memory

## Overview

A URLSessionDataTask is a concrete subclass of URLSessionTask. The methods in the URLSessionDataTask class are documented in URLSessionTask.

A data task returns data directly to the app (in memory) as one or more `NSData` objects. When you use a data task:

- During upload of the body data (if your app provides any), the session periodically calls its delegate’s urlSession(_:task:didSendBodyData:totalBytesSent:totalBytesExpectedToSend:) method with status information.

- After receiving an initial response, the session calls its delegate’s urlSession(_:dataTask:didReceive:completionHandler:) method to let you examine the status code and headers, and optionally convert the data task into a download task.

- During the transfer, the session calls its delegate’s urlSession(_:dataTask:didReceive:) method to provide your app with the content as it arrives.

- Upon completion, the session calls its delegate’s urlSession(_:dataTask:willCacheResponse:completionHandler:) method to let you determine whether the response should be cached.

For examples of using data tasks for fetching and uploading data, see Fetching website data into memory and Uploading data to a website.

## Topics

### Initializers

init()Deprecated

### Type Methods

class func new() -> SelfDeprecated

## Relationships

### Inherits From

- URLSessionTask

### Inherited By

- URLSessionUploadTask

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

### Adding data tasks to a session

func dataTask(with: URL) -> URLSessionDataTask

Creates a task that retrieves the contents of the specified URL.

func dataTask(with: URL, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionDataTask

Creates a task that retrieves the contents of the specified URL, then calls a handler upon completion.

func dataTask(with: URLRequest) -> URLSessionDataTask

Creates a task that retrieves the contents of a URL based on the specified URL request object.

func dataTask(with: URLRequest, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionDataTask

Creates a task that retrieves the contents of a URL based on the specified URL request object, and calls a handler upon completion.

protocol URLSessionDataDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to data and upload tasks.

