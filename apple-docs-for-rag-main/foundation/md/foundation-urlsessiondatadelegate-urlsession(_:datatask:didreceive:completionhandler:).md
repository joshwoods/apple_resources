

- Foundation
- URLSessionDataDelegate
-  urlSession(\_:dataTask:didReceive:completionHandler:) 

Instance Method

# urlSession(\_:dataTask:didReceive:completionHandler:)

Tells the delegate that the data task received the initial reply (headers) from the server.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    dataTask: URLSessionDataTask,
    didReceive response: URLResponse,
    completionHandler: @escaping (URLSession.ResponseDisposition) -> Void
)
```

``` source
optional func urlSession(
    _ session: URLSession,
    dataTask: URLSessionDataTask,
    didReceive response: URLResponse
) async -> URLSession.ResponseDisposition
```

## Parameters 

`session`  

The session containing the data task that received an initial reply.

`dataTask`  

The data task that received an initial reply.

`response`  

A URL response object populated with headers.

`completionHandler`  

A completion handler that your code calls to continue a transfer, passing a URLSession.ResponseDisposition constant to indicate whether the transfer should continue as a data task or should become a download task.

- If you pass URLSession.ResponseDisposition.allow, the task continues as a data task.

- If you pass URLSession.ResponseDisposition.cancel, the task is canceled.

- If you pass URLSession.ResponseDisposition.becomeDownload, your delegate’s urlSession(_:dataTask:didBecome:) method is called to provide the new download task that supersedes the current task.

## Mentioned in 

Fetching website data into memory

## Discussion

Implementing this method is optional unless you need to cancel the transfer or convert it to a download task when the response headers are first received. If you don’t provide this delegate method, the session always allows the task to continue.

You also implement this method if you need to support the fairly obscure `multipart/x-mixed-replace` content type. With that content type, the server sends a series of parts, each of which is intended to replace the previous part. The session calls this method at the beginning of each part, followed by one or more calls to urlSession(_:dataTask:didReceive:) with the contents of that part.

Each time the urlSession(_:dataTask:didReceive:completionHandler:) method is called for a part, collect the data received for the previous part (if any) and process the data as needed for your application. This processing can include storing the data to the filesystem, parsing it into custom types, or displaying it to the user. Next, begin receiving the next part by calling the completion handler with the URLSession.ResponseDisposition.allow constant. Finally, if you have also implemented urlSession(_:task:didCompleteWithError:), the session will call it after sending all the data for the last part.

## See Also

### Handling task life cycle changes

enum ResponseDisposition

Constants indicating how a data or upload session should proceed after receiving the initial headers.

func urlSession(URLSession, dataTask: URLSessionDataTask, didBecome: URLSessionDownloadTask)

Tells the delegate that the data task was changed to a download task.

func urlSession(URLSession, dataTask: URLSessionDataTask, didBecome: URLSessionStreamTask)

Tells the delegate that the data task was changed to a stream task.

