

- Core Location
- CLLocationManager
-  isMonitoringAvailable(for:) 

Type Method

# isMonitoringAvailable(for:)

Returns a Boolean value indicating whether the device supports region monitoring using the specified class.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
class func isMonitoringAvailable(for regionClass: AnyClass) -> Bool
```

## Parameters 

`regionClass`  

A region monitoring class from the MapKit framework. This class must descend from the CLRegion class.

## Return Value

true if the device is capable of monitoring regions using the specified class or false if it is not.

## Discussion

The availability of region monitoring support is dependent on the hardware present on the device. This method does not take into account the availability of location services or the fact that the user might have disabled them for the app or system; you must determine your app’s authorization status separately.

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

class func isRangingAvailable() -> Bool

Returns a Boolean value indicating whether the device supports ranging of beacons that use the iBeacon protocol.

class func locationServicesEnabled() -> Bool

Returns a Boolean value indicating whether location services are enabled on the device.

