

- StoreKit
- SKDownload
-  timeRemaining Deprecated

Instance Property

# timeRemaining

An estimated time, in seconds, to finish downloading the content.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var timeRemaining: TimeInterval { get }
```

Deprecated

Hosted content is no longer supported

## Mentioned in 

Unlocking purchased content

## Discussion

The system attempts to estimate how long it will take to finish downloading the file. If it cannot create a good estimate, the value of this property is set to SKDownloadTimeRemainingUnknown.

## See Also

### Getting State Information

var state: SKDownloadState

The current state of the download object.

Deprecated

var progress: Float

A value that indicates how much of the file has been downloaded.

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

