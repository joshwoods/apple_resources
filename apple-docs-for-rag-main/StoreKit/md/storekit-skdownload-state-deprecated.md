

- StoreKit
- SKDownload
-  state Deprecated

Instance Property

# state

The current state of the download object.

iOS 12.0–16.0DeprecatediPadOS 12.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 12.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var state: SKDownloadState { get }
```

Deprecated

Hosted content is no longer supported

## Discussion

After you queue a download object, the payment queue object calls your transaction observer when the state of the download object changes. Your transaction observer should read the state property and use it to determine how to proceed. For more information on the different states, see SKDownloadState.

## See Also

### Getting State Information

var progress: Float

A value that indicates how much of the file has been downloaded.

Deprecated

var timeRemaining: TimeInterval

An estimated time, in seconds, to finish downloading the content.

Deprecated

var SKDownloadTimeRemainingUnknown: TimeInterval

Indicates that the system cannot determine how much time is needed to finish downloading the content.

Deprecated

enum SKDownloadState

The states that a download operation can be in.

Deprecated

var downloadState: SKDownloadState

The current state of the download object.

Deprecated

