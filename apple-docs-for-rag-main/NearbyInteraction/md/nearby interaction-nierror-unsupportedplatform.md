

- Nearby Interaction
- NIError
-  unsupportedPlatform 

Type Property

# unsupportedPlatform

An error code that indicates that the framework doesn’t support the device platform.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
static var unsupportedPlatform: NIError.Code { get }
```

## Discussion

Before running an interaction session, call isSupported to ensure that Nearby Interaction supports the device’s platform.

## See Also

### Identifying an error cause

enum Code

Codes that identify errors in Nearby Interaction.

static var activeSessionsLimitExceeded: NIError.Code

An error code that indicates that the app reached the maximum number of sessions.

static var invalidConfiguration: NIError.Code

An error code that indicates that the nearby-interaction configuration isn’t valid.

static var resourceUsageTimeout: NIError.Code

An error code that indicates that the framework timed out the session.

static var sessionFailed: NIError.Code

An error code that indicates that the session failed.

static var userDidNotAllow: NIError.Code

An error code that indicates that the user declined the request to share their relative position with nearby devices.

static var invalidARConfiguration: NIError.Code

An error that indicates the framework can’t begin Camera Assistance.

static var activeExtendedDistanceSessionsLimitExceeded: NIError.Code

An error code that indicates that the device exceeds the available number of active extended distance sessions.

static var incompatiblePeerDevice: NIError.Code

An error that indicates the peer device isn’t compatible with this Nearby Interaction session instance.

static var accessoryPeerDeviceUnavailable: NIError.Code

An error that indicates the peer Bluetooth accessory isn’t connected or paired.

