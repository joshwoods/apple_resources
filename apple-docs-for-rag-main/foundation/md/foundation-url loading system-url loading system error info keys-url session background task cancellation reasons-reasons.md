

- Foundation
- URL Loading System
- URL Loading System error info keys
-  URL Session Background Task Cancellation Reasons 

API Collection

# URL Session Background Task Cancellation Reasons

Reasons that indicate why the system canceled a background task.

## Topics

### Cancellation reasons

var NSURLErrorCancelledReasonBackgroundUpdatesDisabled: Int

A reason that indicates the system canceled the background task because background tasks are disabled.

var NSURLErrorCancelledReasonInsufficientSystemResources: Int

A reason that indicates the system canceled the background task because it lacks sufficient resources to perform the task.

var NSURLErrorCancelledReasonUserForceQuitApplication: Int

A reason that indicates the system canceled the background task because the user force-quit the application.

## See Also

### Keys

let NSURLErrorFailingURLErrorKey: String

The URL which caused a load to fail.

let NSURLErrorFailingURLPeerTrustErrorKey: String

The state of a failed SSL handshake.

let NSURLErrorFailingURLStringErrorKey: String

The URL which caused a load to fail.

Deprecated

let NSURLErrorBackgroundTaskCancelledReasonKey: String

A key in the error dictionary that provides the reason for canceling a background task.

let NSURLErrorNetworkUnavailableReasonKey: String

The reason the network was unavailable for a task.

enum NetworkUnavailableReason

An enumeration of reasons explaining why a task couldn’t satisfy networking constraints.

