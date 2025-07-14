

- Nearby Interaction
- NIError
- NIError.Code
-  NIError.Code.resourceUsageTimeout 

Case

# NIError.Code.resourceUsageTimeout

An error code that indicates that the framework timed out the session.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
case resourceUsageTimeout
```

## Discussion

The framework times out a session in some cases to preserve resources, such as battery life. An app needs to watch for timed-out peers. If the app wishes to continue interaction with a timed-out peer device, the app needs to begin a new nearby-interaction session.

## See Also

### Errors

case activeSessionsLimitExceeded

An error code that indicates that the app reached the maximum number of sessions.

case invalidConfiguration

An error code that indicates that the nearby-interaction configuration isn’t valid.

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

