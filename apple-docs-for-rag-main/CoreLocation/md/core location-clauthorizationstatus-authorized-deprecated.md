

- Core Location
- CLAuthorizationStatus
-  authorized Deprecated

Type Property

# authorized

The user authorized the app to use location services.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6+

``` source
static var authorized: CLAuthorizationStatus { get }
```

Deprecated

For iOS, use CLAuthorizationStatus.authorizedAlways or CLAuthorizationStatus.authorizedWhenInUse instead.

## See Also

### Getting the authorization status

case notDetermined

The user has not chosen whether the app can use location services.

case restricted

The app is not authorized to use location services.

case denied

The user denied the use of location services for the app or they are disabled globally in Settings.

case authorizedAlways

The user authorized the app to start location services at any time.

case authorizedWhenInUse

The user authorized the app to start location services while it is in use.

