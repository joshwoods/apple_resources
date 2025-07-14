

- Nearby Interaction
- NIError
- NIError.Code
-  NIError.Code.unsupportedPlatform 

Case

# NIError.Code.unsupportedPlatform

An error code that indicates that the framework doesn’t support the device platform.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
case unsupportedPlatform
```

## Discussion

Before running an interaction session, call isSupported to ensure that Nearby Interaction supports the device’s platform.

## See Also

### Errors

case activeSessionsLimitExceeded

An error code that indicates that the app reached the maximum number of sessions.

case invalidConfiguration

An error code that indicates that the nearby-interaction configuration isn’t valid.

case resourceUsageTimeout

An error code that indicates that the framework timed out the session.

case sessionFailed

An error code that indicates that the session failed.

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

