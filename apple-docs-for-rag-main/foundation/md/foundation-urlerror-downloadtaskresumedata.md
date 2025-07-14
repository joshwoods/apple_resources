

- Foundation
- URLError
-  downloadTaskResumeData 

Instance Property

# downloadTaskResumeData

An opaque data object used to resume a failed download task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var downloadTaskResumeData: Data? { get }
```

## Discussion

Pass this object to downloadTask(withResumeData:) or downloadTask(withResumeData:completionHandler:) to create a new download task that can attempt to resume the failed download.

## See Also

### Error details

var failingURL: URL?

The URL which caused a load to fail.

var failureURLPeerTrust: SecTrust?

The state of a failed SSL handshake.

var failureURLString: String?

The string for the URL which caused a load to fail.

Deprecated

var backgroundTaskCancelledReason: URLError.BackgroundTaskCancelledReason?

The reason for canceling a background task.

enum BackgroundTaskCancelledReason

An enumeration of reasons used to explain the cancellation of a background task.

var networkUnavailableReason: URLError.NetworkUnavailableReason?

The reason the network was unavailable for a task.

enum NetworkUnavailableReason

An enumeration of reasons explaining why a task couldn’t satisfy networking constraints.

