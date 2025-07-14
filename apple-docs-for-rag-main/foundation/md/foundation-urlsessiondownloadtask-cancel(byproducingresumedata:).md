

- Foundation
- URLSessionDownloadTask
-  cancel(byProducingResumeData:) 

Instance Method

# cancel(byProducingResumeData:)

Cancels a download and calls a callback with resume data for later use.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cancel(byProducingResumeData completionHandler: @escaping (Data?) -> Void)
```

``` source
func cancelByProducingResumeData() async -> Data?
```

## Parameters 

`completionHandler`  

A completion handler that is called when the download has been successfully canceled.

If the download is resumable, the completion handler is provided with a `resumeData` object. Your app can later pass this object to a session’s downloadTask(withResumeData:) or downloadTask(withResumeData:completionHandler:) method to create a new task that resumes the download where it left off.

This block is not guaranteed to execute in a particular thread context. As such, you may want specify an appropriate dispatch queue in which to perform any work.

## Mentioned in 

Pausing and resuming downloads

Pausing and resuming uploads

## Discussion

A download can be resumed only if the following conditions are met:

- The resource has not changed since you first requested it

- The task is an HTTP or HTTPS `GET` request

- The server provides either the `ETag` or `Last-Modified` header (or both) in its response

- The server supports byte-range requests

- The temporary file hasn’t been deleted by the system in response to disk space pressure

