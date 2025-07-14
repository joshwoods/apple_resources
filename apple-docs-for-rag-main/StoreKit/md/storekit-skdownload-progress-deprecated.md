

- StoreKit
- SKDownload
-  progress Deprecated

Instance Property

# progress

A value that indicates how much of the file has been downloaded.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var progress: Float { get }
```

Deprecated

Hosted content is no longer supported

## Mentioned in 

Unlocking purchased content

## Discussion

The value of this property is a floating point number between `0.0` and `1.0`, inclusive, where `0.0` means no data has been download and `1.0` means all the data has been downloaded. Typically, your app uses the value of this property to update a user interface element, such as a progress bar, that displays how much of the file has been downloaded.

Do not use the value of this property to determine whether the download has completed. Instead, use the downloadState property.

## See Also

### Getting State Information

var state: SKDownloadState

The current state of the download object.

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

