

- App Tracking Transparency
- ATTrackingManager
-  ATTrackingManager.AuthorizationStatus 

Enumeration

# ATTrackingManager.AuthorizationStatus

The status values for app tracking authorization.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum AuthorizationStatus
```

## Overview

After a device receives an authorization request to approve access to app-related data that can be used for tracking the user or the device, the returned value is either:

- ATTrackingManager.AuthorizationStatus.authorized, or

- ATTrackingManager.AuthorizationStatus.denied.

Before a device receives an authorization request to approve access to app-related data that can be used for tracking the user or the device, the returned value is: ATTrackingManager.AuthorizationStatus.notDetermined.

If authorization to use app tracking data is restricted, the value is: ATTrackingManager.AuthorizationStatus.restricted.

## Topics

### Cases

case authorized

The value that returns if the user authorizes access to app-related data for tracking the user or the device.

case denied

The value that returns if the user denies authorization to access app-related data for tracking the user or the device.

case notDetermined

The value that returns when the app can’t determine the user’s authorization status for access to app-related data for tracking the user or the device.

case restricted

The value that returns if authorization to access app-related data for tracking the user or the device has a restricted status.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining Tracking Authorization Status

class var trackingAuthorizationStatus: ATTrackingManager.AuthorizationStatus

The authorization status that is current for the calling application.

