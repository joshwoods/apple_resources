

- Foundation
- URLSessionDownloadDelegate
-  urlSession(\_:downloadTask:didResumeAtOffset:expectedTotalBytes:) 

Instance Method

# urlSession(\_:downloadTask:didResumeAtOffset:expectedTotalBytes:)

Tells the delegate that the download task has resumed downloading.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    downloadTask: URLSessionDownloadTask,
    didResumeAtOffset fileOffset: Int64,
    expectedTotalBytes: Int64
)
```

## Parameters 

`session`  

The session containing the download task that finished.

`downloadTask`  

The download task that resumed. See explanation in the discussion.

`fileOffset`  

If the file’s cache policy or last modified date prevents reuse of the existing content, then this value is zero. Otherwise, this value is an integer representing the number of bytes on disk that do not need to be retrieved again.

Note

In some situations, it may be possible for the transfer to resume earlier in the file than where the previous transfer ended.

`expectedTotalBytes`  

The expected length of the file, as provided by the `Content-Length` header. If this header was not provided, the value is NSURLSessionTransferSizeUnknown.

## Mentioned in 

Pausing and resuming downloads

## Discussion

If a resumable download task is canceled or fails, you can request a `resumeData` object that provides enough information to restart the download in the future. Later, you can call downloadTask(withResumeData:) or downloadTask(withResumeData:completionHandler:) with that data.

When you call those methods, you get a new download task. As soon as you resume that task, the session calls this method with that new task to indicate that the download is resumed.

