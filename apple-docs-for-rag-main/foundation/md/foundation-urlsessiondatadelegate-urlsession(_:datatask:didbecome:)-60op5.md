

- Foundation
- URLSessionDataDelegate
-  urlSession(\_:dataTask:didBecome:) 

Instance Method

# urlSession(\_:dataTask:didBecome:)

Tells the delegate that the data task was changed to a download task.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    dataTask: URLSessionDataTask,
    didBecome downloadTask: URLSessionDownloadTask
)
```

## Parameters 

`session`  

The session containing the task that was replaced by a download task.

`dataTask`  

The data task that was replaced by a download task.

`downloadTask`  

The new download task that replaced the data task.

## Discussion

When your urlSession(_:dataTask:didReceive:completionHandler:) delegate method uses the URLSession.ResponseDisposition.becomeDownload disposition to convert the request to use a download, the session calls this delegate method to provide you with the new download task. After this call, the session delegate receives no further delegate method calls related to the original data task.

## See Also

### Handling task life cycle changes

func urlSession(URLSession, dataTask: URLSessionDataTask, didReceive: URLResponse, completionHandler: (URLSession.ResponseDisposition) -> Void)

Tells the delegate that the data task received the initial reply (headers) from the server.

enum ResponseDisposition

Constants indicating how a data or upload session should proceed after receiving the initial headers.

func urlSession(URLSession, dataTask: URLSessionDataTask, didBecome: URLSessionStreamTask)

Tells the delegate that the data task was changed to a stream task.

