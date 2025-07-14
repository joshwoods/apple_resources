

- Foundation
- URLError
-  failureURLPeerTrust 

Instance Property

# failureURLPeerTrust

The state of a failed SSL handshake.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var failureURLPeerTrust: SecTrust? { get }
```

## See Also

### Error details

var failingURL: URL?

The URL which caused a load to fail.

var failureURLString: String?

The string for the URL which caused a load to fail.

Deprecated

var downloadTaskResumeData: Data?

An opaque data object used to resume a failed download task.

var backgroundTaskCancelledReason: URLError.BackgroundTaskCancelledReason?

The reason for canceling a background task.

enum BackgroundTaskCancelledReason

An enumeration of reasons used to explain the cancellation of a background task.

var networkUnavailableReason: URLError.NetworkUnavailableReason?

The reason the network was unavailable for a task.

enum NetworkUnavailableReason

An enumeration of reasons explaining why a task couldn’t satisfy networking constraints.

