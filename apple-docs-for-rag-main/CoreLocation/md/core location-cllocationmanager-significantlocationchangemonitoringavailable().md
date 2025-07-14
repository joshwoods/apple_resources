

- Core Location
- CLLocationManager
-  significantLocationChangeMonitoringAvailable() 

Type Method

# significantLocationChangeMonitoringAvailable()

Returns a Boolean value indicating whether the significant-change location service is available on the device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
class func significantLocationChangeMonitoringAvailable() -> Bool
```

## Return Value

true if location change monitoring is available; false if it is not.

## Discussion

This method indicates whether the device is able to report updates based on significant location changes only. This capability provides tremendous power savings for apps that want to track a user’s approximate location and don’t need highly accurate position information.

## See Also

### Determining the availability of services

class func headingAvailable() -> Bool

Returns a Boolean value indicating whether the location manager is able to generate heading-related events.

var isAuthorizedForWidgetUpdates: Bool

A Boolean value that indicates whether a widget is eligible to receive location updates.

var accuracyAuthorization: CLAccuracyAuthorization

A value that indicates the level of location accuracy the app has permission to use.

class func isMonitoringAvailable(for: AnyClass) -> Bool

Returns a Boolean value indicating whether the device supports region monitoring using the specified class.

class func isRangingAvailable() -> Bool

Returns a Boolean value indicating whether the device supports ranging of beacons that use the iBeacon protocol.

class func locationServicesEnabled() -> Bool

Returns a Boolean value indicating whether location services are enabled on the device.

