

- Core Location
- CLLocationManager
-  headingAvailable() 

Type Method

# headingAvailable()

Returns a Boolean value indicating whether the location manager is able to generate heading-related events.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+watchOS 2.0+

``` source
class func headingAvailable() -> Bool
```

## Return Value

true if heading data is available; false if it is not.

## Mentioned in 

Configuring your app to use location services

## Discussion

Heading data may not be available on all iOS-based devices. You should check the value returned by this method before asking the location manager to deliver heading-related events.

## See Also

### Determining the availability of services

class func significantLocationChangeMonitoringAvailable() -> Bool

Returns a Boolean value indicating whether the significant-change location service is available on the device.

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

