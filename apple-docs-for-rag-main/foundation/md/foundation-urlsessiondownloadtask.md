

- Foundation
-  URLSessionDownloadTask 

Class

# URLSessionDownloadTask

A URL session task that stores downloaded data to a file.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class URLSessionDownloadTask
```

## Mentioned in 

Pausing and resuming downloads

Downloading files from websites

Fetching website data into memory

## Overview

An URLSessionDownloadTask is a concrete subclass of URLSessionTask, which provides most of the methods for this class.

Download tasks directly write the server’s response data to a temporary file, providing your app with progress updates as data arrives from the server. When you use download tasks in background sessions, these downloads continue even when your app is in the suspended state or otherwise not running.

You can pause (cancel) download tasks and resume them later (assuming the server supports doing so). You can also resume downloads that failed because of network connectivity problems.

### Download delegate behavior

When you use a download task, your delegate receives several callbacks unique to download scenarios.

- During download, the session periodically calls the delegate’s urlSession(_:downloadTask:didWriteData:totalBytesWritten:totalBytesExpectedToWrite:) method with status information.

- Upon successful completion, the session calls the delegate’s urlSession(_:downloadTask:didFinishDownloadingTo:) method or completion handler. In that method, you must either open the file for reading or move it to a permanent location in your app’s sandbox container directory.

- Upon unsuccessful completion, the session calls the delegate’s urlSession(_:task:didCompleteWithError:) method or completion handler. The only errors your delegate receives through the `error` parameter are client-side errors, such as being unable to resolve the hostname or connect to the host. To check for server-side errors, inspect the response property of the `task` parameter received by this callback.

## Topics

### Canceling a download

func cancel(byProducingResumeData: (Data?) -> Void)

Cancels a download and calls a callback with resume data for later use.

### Creating download tasks

init()

Initializes a download task.

Deprecated

class func new() -> Self

Creates and initializes a download task.

Deprecated

## Relationships

### Inherits From

- URLSessionTask

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- ProgressReporting
- Sendable

## See Also

### Adding download tasks to a session

func downloadTask(with: URL) -> URLSessionDownloadTask

Creates a download task that retrieves the contents of the specified URL and saves the results to a file.

func downloadTask(with: URL, completionHandler: (URL?, URLResponse?, (any Error)?) -> Void) -> URLSessionDownloadTask

Creates a download task that retrieves the contents of the specified URL, saves the results to a file, and calls a handler upon completion.

func downloadTask(with: URLRequest) -> URLSessionDownloadTask

Creates a download task that retrieves the contents of a URL based on the specified URL request object and saves the results to a file.

func downloadTask(with: URLRequest, completionHandler: (URL?, URLResponse?, (any Error)?) -> Void) -> URLSessionDownloadTask

Creates a download task that retrieves the contents of a URL based on the specified URL request object, saves the results to a file, and calls a handler upon completion.

func downloadTask(withResumeData: Data) -> URLSessionDownloadTask

Creates a download task to resume a previously canceled or failed download.

func downloadTask(withResumeData: Data, completionHandler: (URL?, URLResponse?, (any Error)?) -> Void) -> URLSessionDownloadTask

Creates a download task to resume a previously canceled or failed download and calls a handler upon completion.

protocol URLSessionDownloadDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to download tasks.

