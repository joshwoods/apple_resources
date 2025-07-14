

- Core Location
- CLAuthorizationStatus
-  CLAuthorizationStatus.denied 

Case

# CLAuthorizationStatus.denied

The user denied the use of location services for the app or they are disabled globally in Settings.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case denied
```

## Discussion

When the authorization status is denied, your app can’t use location services. The status can be denied when:

- The user denied location permissions for your app.

- The user turned off location services for the device in Settings.

- Location services are unavailable because the device is in Airplane mode.

If the user re-enables location services in Settings, your app’s authorization returns to its previous state. The status change is reported to your delegate’s locationManager(_:didChangeAuthorization:) method.

You may call locationServicesEnabled() if you wish to determine whether location services are available globally on the device.

## See Also

### Getting the authorization status

case notDetermined

The user has not chosen whether the app can use location services.

case restricted

The app is not authorized to use location services.

static var authorized: CLAuthorizationStatus

The user authorized the app to use location services.

Deprecated

case authorizedAlways

The user authorized the app to start location services at any time.

case authorizedWhenInUse

The user authorized the app to start location services while it is in use.

