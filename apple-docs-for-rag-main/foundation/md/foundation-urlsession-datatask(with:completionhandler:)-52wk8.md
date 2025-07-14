

- Foundation
- URLSession
-  dataTask(with:completionHandler:) 

Instance Method

# dataTask(with:completionHandler:)

Creates a task that retrieves the contents of the specified URL, then calls a handler upon completion.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dataTask(
    with url: URL,
    completionHandler: @escaping (Data?, URLResponse?, (any Error)?) -> Void
) -> URLSessionDataTask
```

## Parameters 

`url`  

The URL to be retrieved.

`completionHandler`  

The completion handler to call when the load request is complete. This handler is executed on the delegate queue.

If you pass `nil`, only the session delegate methods are called when the task completes, making this method equivalent to the dataTask(with:) method.

This completion handler takes the following parameters:

`data`  
The data returned by the server.

`response`  
An object that provides response metadata, such as HTTP headers and status code. If you are making an HTTP or HTTPS request, the returned object is actually an HTTPURLResponse object.

`error`  
An error object that indicates why the request failed, or `nil` if the request was successful.

## Return Value

The new session data task.

## Mentioned in 

Processing URL session data task results with Combine

## Discussion

After you create the task, you must start it by calling its resume() method.

By using the completion handler, the task bypasses calls to delegate methods for response and data delivery, and instead provides any resulting NSData, URLResponse, and NSError objects inside the completion handler. Delegate methods for handling authentication challenges, however, are still called.

You should pass a `nil` completion handler *only* when creating tasks in sessions whose delegates include a urlSession(_:dataTask:didReceive:) method.

If the request completes successfully, the `data` parameter of the completion handler block contains the resource data, and the `error` parameter is `nil`. If the request fails, the `data` parameter is `nil` and the `error` parameter contain information about the failure. If a response from the server is received, regardless of whether the request completes successfully or fails, the `response` parameter contains that information.

## See Also

### Adding data tasks to a session

func dataTask(with: URL) -> URLSessionDataTask

Creates a task that retrieves the contents of the specified URL.

func dataTask(with: URLRequest) -> URLSessionDataTask

Creates a task that retrieves the contents of a URL based on the specified URL request object.

func dataTask(with: URLRequest, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionDataTask

Creates a task that retrieves the contents of a URL based on the specified URL request object, and calls a handler upon completion.

class URLSessionDataTask

A URL session task that returns downloaded data directly to the app in memory.

protocol URLSessionDataDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to data and upload tasks.

