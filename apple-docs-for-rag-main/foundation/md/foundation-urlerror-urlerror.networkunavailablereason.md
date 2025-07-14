

- Foundation
- URLError
-  URLError.NetworkUnavailableReason 

Enumeration

# URLError.NetworkUnavailableReason

An enumeration of reasons explaining why a task couldn’t satisfy networking constraints.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum NetworkUnavailableReason
```

## Overview

The network may be unavailable due to restrictions placed on the URLSessionConfiguration, such as allowsConstrainedNetworkAccess, allowsExpensiveNetworkAccess and allowsCellularAccess.

## Topics

### Unavailability reasons

case cellular

A reason that indicates network is unavailable because the interface is cellular and cellular network is disabled.

case constrained

A reason that indicates network is unavailable because the user enabled “Low Data Mode” in the Settings app.

case expensive

A reason that indicates network is unavailable because the system marked the interface as expensive.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var backgroundTaskCancelledReason: URLError.BackgroundTaskCancelledReason?

The reason for canceling a background task.

enum BackgroundTaskCancelledReason

An enumeration of reasons used to explain the cancellation of a background task.

var networkUnavailableReason: URLError.NetworkUnavailableReason?

The reason the network was unavailable for a task.

