

- Nearby Interaction
- NIError
- NIError.Code
-  NIError.Code.invalidARConfiguration 

Case

# NIError.Code.invalidARConfiguration

An error that indicates the framework can’t begin Camera Assistance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
case invalidARConfiguration
```

## Discussion

The framework invalidates a Nearby Interaction session when the app requests Camera Assistance (isCameraAssistanceEnabled) and either of the following are true:

- The device doesn’t support Camera Assistance.

- The app’s AR session doesn’t meet the required criteria as defined in setARSession(_:).

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

case unsupportedPlatform

An error code that indicates that the framework doesn’t support the device platform.

case userDidNotAllow

An error code that indicates that the user declined the request to share their relative position with nearby devices.

case accessoryPeerDeviceUnavailable

An error that indicates the peer Bluetooth accessory isn’t connected or paired.

case incompatiblePeerDevice

An error that indicates the peer device isn’t compatible with this Nearby Interaction session instance.

case activeExtendedDistanceSessionsLimitExceeded

An error that indicates the device exceeds the available number of active extended distance sessions.

