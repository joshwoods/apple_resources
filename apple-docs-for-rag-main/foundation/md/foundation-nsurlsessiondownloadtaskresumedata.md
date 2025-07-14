

- Foundation
-  NSURLSessionDownloadTaskResumeData 

Global Variable

# NSURLSessionDownloadTaskResumeData

A key in the error dictionary that provides resume data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSURLSessionDownloadTaskResumeData: String
```

## Mentioned in 

Pausing and resuming downloads

## Discussion

When a transfer error occurs or when you call the cancel(byProducingResumeData:) method, the delegate object or completion handler gets an NSError object. If the transfer is resumable, that error object’s `userInfo` dictionary contains a value for this key. To resume the transfer, your app can pass that value to the downloadTask(withResumeData:) or downloadTask(withResumeData:completionHandler:) method.

## See Also

### User info dictionary keys

let NSURLErrorBackgroundTaskCancelledReasonKey: String

A key in the error dictionary that provides the reason for canceling a background task.

