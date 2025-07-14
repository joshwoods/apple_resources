

- Core Location
- CLLocationManager
-  isRangingAvailable() 

Type Method

# isRangingAvailable()

Returns a Boolean value indicating whether the device supports ranging of beacons that use the iBeacon protocol.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class func isRangingAvailable() -> Bool
```

## Return Value

true if the device supports ranging or false if it does not.

## See Also

### Determining the availability of services

class func significantLocationChangeMonitoringAvailable() -> Bool

Returns a Boolean value indicating whether the significant-change location service is available on the device.

class func headingAvailable() -> Bool

Returns a Boolean value indicating whether the location manager is able to generate heading-related events.

var isAuthorizedForWidgetUpdates: Bool

A Boolean value that indicates whether a widget is eligible to receive location updates.

var accuracyAuthorization: CLAccuracyAuthorization

A value that indicates the level of location accuracy the app has permission to use.

class func isMonitoringAvailable(for: AnyClass) -> Bool

Returns a Boolean value indicating whether the device supports region monitoring using the specified class.

class func locationServicesEnabled() -> Bool

Returns a Boolean value indicating whether location services are enabled on the device.

