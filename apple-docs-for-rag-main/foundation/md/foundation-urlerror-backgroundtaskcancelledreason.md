

- Foundation
- URLError
-  backgroundTaskCancelledReason 

Instance Property

# backgroundTaskCancelledReason

The reason for canceling a background task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var backgroundTaskCancelledReason: URLError.BackgroundTaskCancelledReason? { get }
```

## Discussion

If the error doesn’t involve cancellation of a background task, this property is `nil`.

## See Also

### Error details

var failingURL: URL?

The URL which caused a load to fail.

var failureURLPeerTrust: SecTrust?

The state of a failed SSL handshake.

var failureURLString: String?

The string for the URL which caused a load to fail.

Deprecated

var downloadTaskResumeData: Data?

An opaque data object used to resume a failed download task.

enum BackgroundTaskCancelledReason

An enumeration of reasons used to explain the cancellation of a background task.

var networkUnavailableReason: URLError.NetworkUnavailableReason?

The reason the network was unavailable for a task.

enum NetworkUnavailableReason

An enumeration of reasons explaining why a task couldn’t satisfy networking constraints.

