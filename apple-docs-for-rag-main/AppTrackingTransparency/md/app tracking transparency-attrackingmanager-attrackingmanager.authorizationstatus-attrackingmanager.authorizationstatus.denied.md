

- App Tracking Transparency
- ATTrackingManager
- ATTrackingManager.AuthorizationStatus
-  ATTrackingManager.AuthorizationStatus.denied 

Case

# ATTrackingManager.AuthorizationStatus.denied

The value that returns if the user denies authorization to access app-related data for tracking the user or the device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
case denied
```

## Discussion

The end user has denied the authorization request to access app-related data that can be used for tracking the user or the device.

## See Also

### Cases

case authorized

The value that returns if the user authorizes access to app-related data for tracking the user or the device.

case notDetermined

The value that returns when the app can’t determine the user’s authorization status for access to app-related data for tracking the user or the device.

case restricted

The value that returns if authorization to access app-related data for tracking the user or the device has a restricted status.

