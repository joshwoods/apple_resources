

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:didChangeAuthorization:) Deprecated

Instance Method

# locationManager(\_:didChangeAuthorization:)

Tells the delegate its authorization status when the app creates the location manager and when the authorization status changes.

iOS 4.2–14.0DeprecatediPadOS 4.2–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.7–11.0DeprecatedtvOS 9.0–14.0DeprecatedwatchOS 1.0–7.0Deprecated

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    didChangeAuthorization status: CLAuthorizationStatus
)
```

Deprecated

Use locationManagerDidChangeAuthorization(_:) instead.

## Parameters 

`manager`  

The location manager object reporting the event.

`status`  

The authorization status for the app.

## See Also

### Responding to authorization changes

func locationManagerDidChangeAuthorization(CLLocationManager)

Tells the delegate when the app creates the location manager and when the authorization status changes.

