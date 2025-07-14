

- StoreKit
- SKDownload
-  downloadState Deprecated

Instance Property

# downloadState

The current state of the download object.

iOS 6.0–12.0DeprecatediPadOS 6.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–12.0Deprecated

``` source
var downloadState: SKDownloadState { get }
```

## Mentioned in 

Unlocking purchased content

## Discussion

After you queue a download object, the payment queue object calls your transaction observer when the state of the download object changes. Your transaction observer should read the downloadState property and use it to determine how to proceed. For more information on the different states, see SKDownloadState.

## See Also

### Getting State Information

var state: SKDownloadState

The current state of the download object.

Deprecated

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

