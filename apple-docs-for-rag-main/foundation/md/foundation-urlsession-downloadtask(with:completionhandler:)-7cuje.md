

- Foundation
- URLSession
-  downloadTask(with:completionHandler:) 

Instance Method

# downloadTask(with:completionHandler:)

Creates a download task that retrieves the contents of the specified URL, saves the results to a file, and calls a handler upon completion.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func downloadTask(
    with url: URL,
    completionHandler: @escaping (URL?, URLResponse?, (any Error)?) -> Void
) -> URLSessionDownloadTask
```

## Parameters 

`url`  

The URL to download.

`completionHandler`  

The completion handler to call when the load request is complete. This handler is executed on the delegate queue.

If you pass `nil`, only the session delegate methods are called when the task completes, making this method equivalent to the downloadTask(with:) method.

This completion handler takes the following parameters:

`location`  
The location of a temporary file where the server’s response is stored. You must move this file or open it for reading before your completion handler returns. Otherwise, the file is deleted, and the data is lost.

`response`  
An object that provides response metadata, such as HTTP headers and status code. If you are making an HTTP or HTTPS request, the returned object is actually an HTTPURLResponse object.

`error`  
An error object that indicates why the request failed, or `nil` if the request was successful.

## Return Value

The new session download task.

## Discussion

By using the completion handler, the task bypasses calls to delegate methods for response and data delivery, and instead provides any resulting NSData, URLResponse, and NSError objects inside the completion handler. Delegate methods for handling authentication challenges, however, are still called.

You should pass a `nil` completion handler *only* when creating tasks in sessions whose delegates include a urlSession(_:downloadTask:didFinishDownloadingTo:) method.

After you create the task, you must start it by calling its resume() method.

If the request completes successfully, the `location` parameter of the completion handler block contains the location of the temporary file, and the `error` parameter is `nil`. If the request fails, the `location` parameter is `nil` and the `error` parameter contain information about the failure. If a response from the server is received, regardless of whether the request completes successfully or fails, the `response` parameter contains that information.

## See Also

### Adding download tasks to a session

func downloadTask(with: URL) -> URLSessionDownloadTask

Creates a download task that retrieves the contents of the specified URL and saves the results to a file.

func downloadTask(with: URLRequest) -> URLSessionDownloadTask

Creates a download task that retrieves the contents of a URL based on the specified URL request object and saves the results to a file.

func downloadTask(with: URLRequest, completionHandler: (URL?, URLResponse?, (any Error)?) -> Void) -> URLSessionDownloadTask

Creates a download task that retrieves the contents of a URL based on the specified URL request object, saves the results to a file, and calls a handler upon completion.

func downloadTask(withResumeData: Data) -> URLSessionDownloadTask

Creates a download task to resume a previously canceled or failed download.

func downloadTask(withResumeData: Data, completionHandler: (URL?, URLResponse?, (any Error)?) -> Void) -> URLSessionDownloadTask

Creates a download task to resume a previously canceled or failed download and calls a handler upon completion.

class URLSessionDownloadTask

A URL session task that stores downloaded data to a file.

protocol URLSessionDownloadDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to download tasks.

