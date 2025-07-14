

- Core Location
- CLAuthorizationStatus
-  CLAuthorizationStatus.authorizedWhenInUse 

Case

# CLAuthorizationStatus.authorizedWhenInUse

The user authorized the app to start location services while it is in use.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case authorizedWhenInUse
```

## Discussion

This authorization allows you to use all location services and receive location events only when your app is in use. To continue using location services in the background, enable Continuous Background Location Updates and start the services while the app is in use.

## See Also

### Getting the authorization status

case notDetermined

The user has not chosen whether the app can use location services.

case restricted

The app is not authorized to use location services.

case denied

The user denied the use of location services for the app or they are disabled globally in Settings.

static var authorized: CLAuthorizationStatus

The user authorized the app to use location services.

Deprecated

case authorizedAlways

The user authorized the app to start location services at any time.

