

- Foundation
- URLSession
-  uploadTask(with:fromFile:completionHandler:) 

Instance Method

# uploadTask(with:fromFile:completionHandler:)

Creates a task that performs an HTTP request for uploading the specified file, then calls a handler upon completion.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func uploadTask(
    with request: URLRequest,
    fromFile fileURL: URL,
    completionHandler: @escaping (Data?, URLResponse?, (any Error)?) -> Void
) -> URLSessionUploadTask
```

## Parameters 

`request`  

A URL request object that provides the URL, cache policy, request type, and so on. The body stream and body data in this request object are ignored.

`fileURL`  

The URL of the file to upload.

`completionHandler`  

The completion handler to call when the load request is complete. This handler is executed on the delegate queue.

If you pass `nil`, only the session delegate methods are called when the task completes, making this method equivalent to the uploadTask(with:fromFile:) method.

This completion handler takes the following parameters:

`data`  
The data returned by the server.

`response`  
An object that provides response metadata, such as HTTP headers and status code. If you are making an HTTP or HTTPS request, the returned object is actually an HTTPURLResponse object.

`error`  
An error object that indicates why the request failed, or `nil` if the request was successful.

## Return Value

The new session upload task.

## Discussion

An HTTP upload request is any request that contains a request body, such as a `POST` or `PUT` request. Upload tasks require you to create a request object so that you can provide metadata for the upload, like HTTP request headers.

Unlike uploadTask(with:fromFile:), this method returns the response body after it has been received in full, and does not require you to write a custom delegate to obtain the response body.

By using a completion handler, the task bypasses calls to delegate methods for response and data delivery, and instead provides any resulting data, response, or error inside the completion handler. Delegate methods for handling authentication challenges, however, are still called.

Typically you usually pass a `nil` completion handler only when creating tasks in sessions whose delegates include a urlSession(_:dataTask:didReceive:) method. However, if you do not need the response data, use key-value observing to watch for changes to the task’s status to determine when it completes.

After you create the task, you must start it by calling its resume() method.

If the request completes successfully, the `data` parameter of the completion handler block contains the resource data, and the `error` parameter is `nil`. If the request fails, the `data` parameter is `nil,` and the `error` parameter contains information about the failure. If a response from the server is received, regardless of whether the request completes successfully or fails, the `response` parameter contains that information.

## See Also

### Adding upload tasks to a session

func uploadTask(with: URLRequest, from: Data) -> URLSessionUploadTask

Creates a task that performs an HTTP request for the specified URL request object and uploads the provided data.

func uploadTask(with: URLRequest, from: Data?, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionUploadTask

Creates a task that performs an HTTP request for the specified URL request object, uploads the provided data, and calls a handler upon completion.

func uploadTask(with: URLRequest, fromFile: URL) -> URLSessionUploadTask

Creates a task that performs an HTTP request for uploading the specified file.

func uploadTask(withStreamedRequest: URLRequest) -> URLSessionUploadTask

Creates a task that performs an HTTP request for uploading data based on the specified URL request.

func uploadTask(withResumeData: Data) -> URLSessionUploadTask

func uploadTask(withResumeData: Data, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionUploadTask

class URLSessionUploadTask

A URL session task that uploads data to the network in a request body.

protocol URLSessionDataDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to data and upload tasks.

