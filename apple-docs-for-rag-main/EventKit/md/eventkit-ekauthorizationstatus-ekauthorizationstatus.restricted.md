

- EventKit
- EKAuthorizationStatus
-  EKAuthorizationStatus.restricted 

Case

# EKAuthorizationStatus.restricted

The app isn’t authorized to access the service.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+watchOS 2.0+

``` source
case restricted
```

## Discussion

The person can’t change your app’s authorization status, possibly due to active restrictions such as parental controls being in place.

## See Also

### Status

case fullAccess

The app has both read and write access to the requested entity type.

case writeOnly

The app has write-only access to the requested entity type.

case denied

The person explicitly denied access to the service for the app.

case notDetermined

The person hasn’t chosen whether the app may access the service.

