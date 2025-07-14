

- Core Location
- CLAuthorizationStatus
-  CLAuthorizationStatus.restricted 

Case

# CLAuthorizationStatus.restricted

The app is not authorized to use location services.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case restricted
```

## Discussion

The user cannot change this app’s status, possibly due to active restrictions such as parental controls being in place.

## See Also

### Getting the authorization status

case notDetermined

The user has not chosen whether the app can use location services.

case denied

The user denied the use of location services for the app or they are disabled globally in Settings.

static var authorized: CLAuthorizationStatus

The user authorized the app to use location services.

Deprecated

case authorizedAlways

The user authorized the app to start location services at any time.

case authorizedWhenInUse

The user authorized the app to start location services while it is in use.

