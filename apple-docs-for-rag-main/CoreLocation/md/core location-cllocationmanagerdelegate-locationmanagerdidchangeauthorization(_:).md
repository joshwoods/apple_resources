

- Core Location
- CLLocationManagerDelegate
-  locationManagerDidChangeAuthorization(\_:) 

Instance Method

# locationManagerDidChangeAuthorization(\_:)

Tells the delegate when the app creates the location manager and when the authorization status changes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
optional func locationManagerDidChangeAuthorization(_ manager: CLLocationManager)
```

## Parameters 

`manager`  

The location manager object reporting the event.

## Mentioned in 

Requesting authorization to use location services

## Discussion

The system calls this method when the app creates the related object’s CLLocationManager instance, and when the app’s authorization status changes. The status informs the app whether it can access the user’s location.

Use this delegate method to manage your app’s state changes in response to its ability to use location information. For example, you may wish to enable or disable your app’s location-related features, as appropriate. To determine the app’s current authorization, read the new value of the authorizationStatus and accuracyAuthorization properties of the location manager.

Important

Core Location always calls locationManagerDidChangeAuthorization(_:) when the user’s action results in an authorization status change, and when your app creates an instance of CLLocationManager, whether your app runs in the foreground or in the background.

If the user’s choice doesn’t change the authorization status after you call the requestWhenInUseAuthorization() or requestAlwaysAuthorization() method, the location manager doesn’t report the current authorization status to this method—the location manager only reports changes. For example, the location manager calls this method when the status changes from CLAuthorizationStatus.notDetermined to CLAuthorizationStatus.authorizedWhenInUse.

### Events that Cause Authorization Status Changes

An app’s authorization status changes in response to users’ actions. Users can change permission for apps to use location information at any time. The user can:

- Change an app’s location authorization in Settings \> Privacy \> Location Services, or in Settings \> (the app) \> Location Services.

- Turn location services on or off globally in Settings \> Privacy \> Location Services.

- Choose Reset Location & Privacy in Settings \> General \> Reset.

A user’s response to location manager prompts can also change authorization status. For instance, users may change the authorization status by responding to the prompts initiated by calls to requestWhenInUseAuthorization() or requestAlwaysAuthorization() methods. For apps with Always authorization, users may change the authorization status to When In Use when responding to the location usage reminder alert.

When an app has temporary authorization, the authorization changes when the user ceases to use the app.

## See Also

### Responding to authorization changes

func locationManager(CLLocationManager, didChangeAuthorization: CLAuthorizationStatus)

Tells the delegate its authorization status when the app creates the location manager and when the authorization status changes.

Deprecated

