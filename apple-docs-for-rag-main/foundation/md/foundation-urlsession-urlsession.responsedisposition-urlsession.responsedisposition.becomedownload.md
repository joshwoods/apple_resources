

- Foundation
- URLSession
- URLSession.ResponseDisposition
-  URLSession.ResponseDisposition.becomeDownload 

Case

# URLSession.ResponseDisposition.becomeDownload

Convert the response for this request to use a URLSessionDownloadTask.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case becomeDownload
```

## Discussion

When used with the completion handler from urlSession(_:dataTask:didReceive:completionHandler:), this disposition converts the data task to a download task. This will result in your delegate’s urlSession(_:dataTask:didBecome:) being called to provide you with the new download task that supersedes the current task.

## See Also

### Task dispositions

case cancel

Cancel the load.

case allow

Allow the load operation to continue.

case becomeStream

Convert the response for this request to use a URLSessionStreamTask.

