

- Foundation
- URLSessionTaskDelegate
-  urlSession(\_:task:willPerformHTTPRedirection:newRequest:completionHandler:) 

Instance Method

# urlSession(\_:task:willPerformHTTPRedirection:newRequest:completionHandler:)

Tells the delegate that the remote server requested an HTTP redirect.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    task: URLSessionTask,
    willPerformHTTPRedirection response: HTTPURLResponse,
    newRequest request: URLRequest,
    completionHandler: @escaping (URLRequest?) -> Void
)
```

``` source
optional func urlSession(
    _ session: URLSession,
    task: URLSessionTask,
    willPerformHTTPRedirection response: HTTPURLResponse,
    newRequest request: URLRequest
) async -> URLRequest?
```

## Parameters 

`session`  

The session containing the task whose request resulted in a redirect.

`task`  

The task whose request resulted in a redirect.

`response`  

An object containing the server’s response to the original request.

`request`  

A URL request object filled out with the new location.

`completionHandler`  

A block that your handler should call with either the value of the `request` parameter, a modified URL request object, or `NULL` to refuse the redirect and return the body of the redirect response.

## Mentioned in 

Downloading files in the background

## Discussion

This method is called *only* for tasks in default and ephemeral sessions. Tasks in background sessions automatically follow redirects.

