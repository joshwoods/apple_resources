

- Foundation
- URLSession
- URLSession.ResponseDisposition
-  URLSession.ResponseDisposition.cancel 

Case

# URLSession.ResponseDisposition.cancel

Cancel the load.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case cancel
```

## Discussion

Using this disposition is equivalent to calling cancel() on the task.

## See Also

### Task dispositions

case allow

Allow the load operation to continue.

case becomeDownload

Convert the response for this request to use a URLSessionDownloadTask.

case becomeStream

Convert the response for this request to use a URLSessionStreamTask.

