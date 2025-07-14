

- Nearby Interaction
- NIError
- NIError.Code
-  NIError.Code.invalidConfiguration 

Case

# NIError.Code.invalidConfiguration

An error code that indicates that the nearby-interaction configuration isn’t valid.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
case invalidConfiguration
```

## Mentioned in 

Initiating and maintaining a session

## Discussion

The framework invalidates a session with this error code if the app provides an invalid discovery token to the init(peerToken:) initializer.

## See Also

### Errors

case activeSessionsLimitExceeded

An error code that indicates that the app reached the maximum number of sessions.

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

