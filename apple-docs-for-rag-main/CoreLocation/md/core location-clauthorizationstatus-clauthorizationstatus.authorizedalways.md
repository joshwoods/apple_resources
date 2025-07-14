

- Core Location
- CLAuthorizationStatus
-  CLAuthorizationStatus.authorizedAlways 

Case

# CLAuthorizationStatus.authorizedAlways

The user authorized the app to start location services at any time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+watchOS 2.0+

``` source
case authorizedAlways
```

## Mentioned in 

Creating a location push service extension

## Discussion

This authorization allows you to use all location services and receive location events whether or not your app is in use.

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

case authorizedWhenInUse

The user authorized the app to start location services while it is in use.

