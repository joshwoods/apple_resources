

- Foundation
- URLSession
-  downloadTask(with:) 

Instance Method

# downloadTask(with:)

Creates a download task that retrieves the contents of the specified URL and saves the results to a file.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func downloadTask(with url: URL) -> URLSessionDownloadTask
```

## Parameters 

`url`  

The URL to download.

## Return Value

The new session download task.

## Mentioned in 

Downloading files in the background

Downloading files from websites

## Discussion

After you create the task, you must start it by calling its resume() method.

## See Also

### Adding download tasks to a session

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

protocol URLSessionDownloadDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to download tasks.

