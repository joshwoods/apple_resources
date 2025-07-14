

- StoreKit
-  SKDownloadState Deprecated

Enumeration

# SKDownloadState

The states that a download operation can be in.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
@frozen
enum SKDownloadState
```

Deprecated

Hosted content is no longer supported

## Topics

### Constants

case waiting

Indicates that the download has not started yet.

case active

Indicates that the content is currently being downloaded.

case paused

Indicates that your app paused the download.

case finished

Indicates that the content was successfully downloaded.

case failed

Indicates that an error occurred while the file was being downloaded.

case cancelled

Indicates that your app canceled the download.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var downloadState: SKDownloadState

The current state of the download object.

Deprecated

