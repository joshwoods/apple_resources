

- Foundation
- URLSession
- URLSession.ResponseDisposition
-  URLSession.ResponseDisposition.becomeStream 

Case

# URLSession.ResponseDisposition.becomeStream

Convert the response for this request to use a URLSessionStreamTask.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case becomeStream
```

## Discussion

When used with the completion handler from urlSession(_:dataTask:didReceive:completionHandler:), this disposition converts the task to a stream task. This will result in your delegate’s urlSession(_:dataTask:didBecome:) being called to provide you with the new stream task that supersedes the current task.

## See Also

### Task dispositions

case cancel

Cancel the load.

case allow

Allow the load operation to continue.

case becomeDownload

Convert the response for this request to use a URLSessionDownloadTask.

