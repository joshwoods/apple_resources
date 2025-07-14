

- Foundation
-  NSURLErrorBackgroundTaskCancelledReasonKey 

Global Variable

# NSURLErrorBackgroundTaskCancelledReasonKey

A key in the error dictionary that provides the reason for canceling a background task.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSURLErrorBackgroundTaskCancelledReasonKey: String
```

## Discussion

The value associated with this key is an NSNumber. For a list of possible values, see URL Session Background Task Cancellation Reasons.

## See Also

### Keys

let NSURLErrorFailingURLErrorKey: String

The URL which caused a load to fail.

let NSURLErrorFailingURLPeerTrustErrorKey: String

The state of a failed SSL handshake.

let NSURLErrorFailingURLStringErrorKey: String

The URL which caused a load to fail.

Deprecated

URL Session Background Task Cancellation Reasons

Reasons that indicate why the system canceled a background task.

let NSURLErrorNetworkUnavailableReasonKey: String

The reason the network was unavailable for a task.

enum NetworkUnavailableReason

An enumeration of reasons explaining why a task couldn’t satisfy networking constraints.

