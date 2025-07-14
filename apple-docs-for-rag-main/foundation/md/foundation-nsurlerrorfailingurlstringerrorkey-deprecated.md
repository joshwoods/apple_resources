

- Foundation
-  NSURLErrorFailingURLStringErrorKey Deprecated

Global Variable

# NSURLErrorFailingURLStringErrorKey

The URL which caused a load to fail.

iOS 4.0–18.4DeprecatediPadOS 4.0–18.4DeprecatedMac Catalyst 13.1–18.4DeprecatedmacOS 10.6–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
let NSURLErrorFailingURLStringErrorKey: String
```

Deprecated

Use NSURLErrorFailingURLErrorKey instead

## Discussion

The corresponding value is an NSString object.

This constant supersedes NSErrorFailingURLStringKey, which was deprecated starting in macOS 10.6. Both constants refer to the same value for backward-compatibility, but this symbol name has a better prefix.

## See Also

### Keys

let NSURLErrorFailingURLErrorKey: String

The URL which caused a load to fail.

let NSURLErrorFailingURLPeerTrustErrorKey: String

The state of a failed SSL handshake.

let NSURLErrorBackgroundTaskCancelledReasonKey: String

A key in the error dictionary that provides the reason for canceling a background task.

URL Session Background Task Cancellation Reasons

Reasons that indicate why the system canceled a background task.

let NSURLErrorNetworkUnavailableReasonKey: String

The reason the network was unavailable for a task.

enum NetworkUnavailableReason

An enumeration of reasons explaining why a task couldn’t satisfy networking constraints.

