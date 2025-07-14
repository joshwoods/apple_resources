

- Foundation
-  URLSessionDownloadDelegate 

Protocol

# URLSessionDownloadDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to download tasks.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol URLSessionDownloadDelegate : URLSessionTaskDelegate
```

## Mentioned in 

Downloading files from websites

Downloading files in the background

Fetching website data into memory

## Overview

In addition to the methods in this protocol, be sure to implement the methods in the URLSessionTaskDelegate and URLSessionDelegate protocols to handle events common to all task types and session-level events, respectively.

Note

An URLSession object need not have a delegate. If no delegate is assigned, a system-provided delegate is used, and you must provide a completion callback to obtain the data.

## Topics

### Handling download life cycle changes

func urlSession(URLSession, downloadTask: URLSessionDownloadTask, didFinishDownloadingTo: URL)

Tells the delegate that a download task has finished downloading.

**Required**

### Resuming paused downloads

func urlSession(URLSession, downloadTask: URLSessionDownloadTask, didResumeAtOffset: Int64, expectedTotalBytes: Int64)

Tells the delegate that the download task has resumed downloading.

### Receiving progress updates

func urlSession(URLSession, downloadTask: URLSessionDownloadTask, didWriteData: Int64, totalBytesWritten: Int64, totalBytesExpectedToWrite: Int64)

Periodically informs the delegate about the download’s progress.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable
- URLSessionDelegate
- URLSessionTaskDelegate

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

class URLSessionDownloadTask

A URL session task that stores downloaded data to a file.

