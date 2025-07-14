

- Core Location
- CLLocationManager
-  isAuthorizedForWidgetUpdates 

Instance Property

# isAuthorizedForWidgetUpdates

A Boolean value that indicates whether a widget is eligible to receive location updates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var isAuthorizedForWidgetUpdates: Bool { get }
```

## Discussion

This property is `true` when either of the following is true:

- The app’s authorization status is CLAuthorizationStatus.authorizedAlways.

- The app’s authorization status is CLAuthorizationStatus.authorizedWhenInUse and the user agrees to extend the app’s authorization status to widgets.

Note

For apps that use CLAuthorizationStatus.authorizedWhenInUse, after the user agrees to extend an app’s authorization status to widgets, the app’s Location Services settings indicate While Using the App or Widgets as the active access level.

For details about using location information in widgets with CLAuthorizationStatus.authorizedWhenInUse, see Accessing location information in widgets.

## See Also

### Determining the availability of services

class func significantLocationChangeMonitoringAvailable() -> Bool

Returns a Boolean value indicating whether the significant-change location service is available on the device.

class func headingAvailable() -> Bool

Returns a Boolean value indicating whether the location manager is able to generate heading-related events.

var accuracyAuthorization: CLAccuracyAuthorization

A value that indicates the level of location accuracy the app has permission to use.

class func isMonitoringAvailable(for: AnyClass) -> Bool

Returns a Boolean value indicating whether the device supports region monitoring using the specified class.

class func isRangingAvailable() -> Bool

Returns a Boolean value indicating whether the device supports ranging of beacons that use the iBeacon protocol.

class func locationServicesEnabled() -> Bool

Returns a Boolean value indicating whether location services are enabled on the device.

