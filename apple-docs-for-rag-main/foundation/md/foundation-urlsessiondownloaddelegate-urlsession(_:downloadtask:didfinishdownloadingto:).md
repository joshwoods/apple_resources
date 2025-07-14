

- Foundation
- URLSessionDownloadDelegate
-  urlSession(\_:downloadTask:didFinishDownloadingTo:) 

Instance Method

# urlSession(\_:downloadTask:didFinishDownloadingTo:)

Tells the delegate that a download task has finished downloading.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func urlSession(
    _ session: URLSession,
    downloadTask: URLSessionDownloadTask,
    didFinishDownloadingTo location: URL
)
```

**Required**

## Parameters 

`session`  

The session containing the download task that finished.

`downloadTask`  

The download task that finished.

`location`  

A file URL for the temporary file. Because the file is temporary, you must either open the file for reading or move it to a permanent location in your app’s sandbox container directory before returning from this delegate method.

If you choose to open the file for reading, you should do the actual reading in another thread to avoid blocking the delegate queue.

## Mentioned in 

Downloading files from websites

Downloading files in the background

