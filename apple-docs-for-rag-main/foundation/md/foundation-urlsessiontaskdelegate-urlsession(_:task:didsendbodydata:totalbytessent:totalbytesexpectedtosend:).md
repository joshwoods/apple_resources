

- Foundation
- URLSessionTaskDelegate
-  urlSession(\_:task:didSendBodyData:totalBytesSent:totalBytesExpectedToSend:) 

Instance Method

# urlSession(\_:task:didSendBodyData:totalBytesSent:totalBytesExpectedToSend:)

Periodically informs the delegate of the progress of sending body content to the server.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    task: URLSessionTask,
    didSendBodyData bytesSent: Int64,
    totalBytesSent: Int64,
    totalBytesExpectedToSend: Int64
)
```

## Parameters 

`session`  

The session containing the data task.

`task`  

The data task.

`bytesSent`  

The number of bytes sent since the last time this delegate method was called.

`totalBytesSent`  

The total number of bytes sent so far.

`totalBytesExpectedToSend`  

The expected length of the body data. The URL loading system can determine the length of the upload data in three ways:

- From the length of the `NSData` object provided as the upload body.

- From the length of the file on disk provided as the upload body of an upload task (*not* a download task).

- From the `Content-Length` in the request object, if you explicitly set it.

Otherwise, the value is NSURLSessionTransferSizeUnknown (`-1`) if you provided a stream or body data object, or zero (`0`) if you did not.

## Discussion

The `totalBytesSent` and `totalBytesExpectedToSend` parameters are also available as URLSessionTask properties countOfBytesSent and countOfBytesExpectedToSend. Or, since URLSessionTask supports ProgressReporting, you can use the task’s progress property instead, which may be more convenient.

## See Also

### Working with upload tasks

func urlSession(URLSession, task: URLSessionTask, needNewBodyStream: (InputStream?) -> Void)

Tells the delegate when a task requires a new request body stream to send to the remote server.

