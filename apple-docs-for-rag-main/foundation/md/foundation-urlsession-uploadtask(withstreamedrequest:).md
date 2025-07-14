

- Foundation
- URLSession
-  uploadTask(withStreamedRequest:) 

Instance Method

# uploadTask(withStreamedRequest:)

Creates a task that performs an HTTP request for uploading data based on the specified URL request.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func uploadTask(withStreamedRequest request: URLRequest) -> URLSessionUploadTask
```

## Parameters 

`request`  

A URL request object that provides the URL, cache policy, request type, and so on. The body stream and body data in this request object are ignored, and the session calls its delegate’s urlSession(_:task:needNewBodyStream:) method to provide the body data.

## Return Value

The new session upload task.

## Mentioned in 

Uploading streams of data

## Discussion

An HTTP upload request is any request that contains a request body, such as a `POST` or `PUT` request. Upload tasks require you to provide a request object so that you can provide metadata for the upload, such as HTTP request headers.

After you create the task, you must start it by calling its resume() method. The task calls methods on the session’s delegate to provide you with the upload’s progress, response metadata, response data, and so on. The session’s delegate must have a urlSession(_:task:needNewBodyStream:) method that provides the body data to upload.

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

func uploadTask(withResumeData: Data) -> URLSessionUploadTask

func uploadTask(withResumeData: Data, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionUploadTask

class URLSessionUploadTask

A URL session task that uploads data to the network in a request body.

protocol URLSessionDataDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to data and upload tasks.

