

- EventKit
- EKAuthorizationStatus
-  EKAuthorizationStatus.writeOnly 

Case

# EKAuthorizationStatus.writeOnly

The app has write-only access to the requested entity type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
case writeOnly
```

## See Also

### Status

case fullAccess

The app has both read and write access to the requested entity type.

case denied

The person explicitly denied access to the service for the app.

case notDetermined

The person hasn’t chosen whether the app may access the service.

case restricted

The app isn’t authorized to access the service.

