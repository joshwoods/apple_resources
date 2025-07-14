

- Nearby Interaction
- NIError
-  NIError.Code 

Enumeration

# NIError.Code

Codes that identify errors in Nearby Interaction.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
enum Code
```

## Overview

This enumeration uses session(_:didInvalidateWith:) to collect the errors the framework provides to the delegate.

## Topics

### Errors

case activeSessionsLimitExceeded

An error code that indicates that the app reached the maximum number of sessions.

case invalidConfiguration

An error code that indicates that the nearby-interaction configuration isn’t valid.

case resourceUsageTimeout

An error code that indicates that the framework timed out the session.

case sessionFailed

An error code that indicates that the session failed.

case unsupportedPlatform

An error code that indicates that the framework doesn’t support the device platform.

case userDidNotAllow

An error code that indicates that the user declined the request to share their relative position with nearby devices.

case invalidARConfiguration

An error that indicates the framework can’t begin Camera Assistance.

case accessoryPeerDeviceUnavailable

An error that indicates the peer Bluetooth accessory isn’t connected or paired.

case incompatiblePeerDevice

An error that indicates the peer device isn’t compatible with this Nearby Interaction session instance.

case activeExtendedDistanceSessionsLimitExceeded

An error that indicates the device exceeds the available number of active extended distance sessions.

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

### Errors

struct NIError

An error Nearby Interaction reports.

let NIErrorDomain: String

A unique error domain for Nearby Interaction.

