

- Foundation
- URLSessionDataDelegate
-  urlSession(\_:dataTask:didBecome:) 

Instance Method

# urlSession(\_:dataTask:didBecome:)

Tells the delegate that the data task was changed to a stream task.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    dataTask: URLSessionDataTask,
    didBecome streamTask: URLSessionStreamTask
)
```

## Parameters 

`session`  

The session containing the task that was replaced by a stream task.

`dataTask`  

The data task that was replaced by a stream task.

`streamTask`  

The new stream task that replaced the data task.

## Discussion

When your urlSession(_:dataTask:didReceive:completionHandler:) delegate method uses the URLSession.ResponseDisposition.becomeStream disposition to convert the request to use a stream, the session calls this delegate method to provide you with the new stream task. After this call, the session delegate receives no further delegate method calls related to the original data task.

For requests that were pipelined, the stream task allows only reading, and the object immediately sends the delegate message urlSession(_:writeClosedFor:). You can disable pipelining for all requests in a session by setting the httpShouldUsePipelining property on its URLSessionConfiguration object, or for individual requests by setting the httpShouldUsePipelining property on an NSURLRequest object.

## See Also

### Handling task life cycle changes

func urlSession(URLSession, dataTask: URLSessionDataTask, didReceive: URLResponse, completionHandler: (URLSession.ResponseDisposition) -> Void)

Tells the delegate that the data task received the initial reply (headers) from the server.

enum ResponseDisposition

Constants indicating how a data or upload session should proceed after receiving the initial headers.

func urlSession(URLSession, dataTask: URLSessionDataTask, didBecome: URLSessionDownloadTask)

Tells the delegate that the data task was changed to a download task.

