

- Foundation
-  URLSessionUploadTask 

Class

# URLSessionUploadTask

A URL session task that uploads data to the network in a request body.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class URLSessionUploadTask
```

## Mentioned in 

Pausing and resuming uploads

Uploading streams of data

Uploading data to a website

## Overview

The URLSessionUploadTask class is a subclass of URLSessionDataTask, which in turn is a concrete subclass of URLSessionTask. The methods associated with the URLSessionUploadTask class are documented in URLSessionTask.

Upload tasks are used for making HTTP requests that require a request body (such as `POST` or `PUT`). They behave similarly to data tasks, but you create them by calling different methods on the session that are designed to make it easier to provide the content to upload. As with data tasks, if the server provides a response, upload tasks return that response as one or more `NSData` objects in memory.

Note

Unlike data tasks, you can use upload tasks to upload content in the background.

When you create an upload task, you provide a URLRequest instance that contains any additional headers that you might need to send alongside the upload, such as the content type, content disposition, and so on. In iOS, when you create an upload task for a file in a background session, the system copies that file to a temporary location and streams data from there.

While the upload is in progress, the task calls the session delegate’s urlSession(_:task:didSendBodyData:totalBytesSent:totalBytesExpectedToSend:) method periodically to provide you with status information.

When the upload phase of the request finishes, the task behaves like a data task, calling methods on the session delegate to provide you with the server’s response—headers, status code, content data, and so on.

## Topics

### Initializers

init()Deprecated

### Instance Methods

func cancel(byProducingResumeData: (Data?) -> Void)

### Type Methods

class func new() -> SelfDeprecated

## Relationships

### Inherits From

- URLSessionDataTask

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

### Adding upload tasks to a session

func uploadTask(with: URLRequest, from: Data) -> URLSessionUploadTask

Creates a task that performs an HTTP request for the specified URL request object and uploads the provided data.

func uploadTask(with: URLRequest, from: Data?, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionUploadTask

Creates a task that performs an HTTP request for the specified URL request object, uploads the provided data, and calls a handler upon completion.

func uploadTask(with: URLRequest, fromFile: URL) -> URLSessionUploadTask

Creates a task that performs an HTTP request for uploading the specified file.

func uploadTask(with: URLRequest, fromFile: URL, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionUploadTask

Creates a task that performs an HTTP request for uploading the specified file, then calls a handler upon completion.

func uploadTask(withStreamedRequest: URLRequest) -> URLSessionUploadTask

Creates a task that performs an HTTP request for uploading data based on the specified URL request.

func uploadTask(withResumeData: Data) -> URLSessionUploadTask

func uploadTask(withResumeData: Data, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionUploadTask

protocol URLSessionDataDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to data and upload tasks.

