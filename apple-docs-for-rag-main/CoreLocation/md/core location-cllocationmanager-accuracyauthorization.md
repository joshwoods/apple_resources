

- Core Location
- CLLocationManager
-  accuracyAuthorization 

Instance Property

# accuracyAuthorization

A value that indicates the level of location accuracy the app has permission to use.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var accuracyAuthorization: CLAccuracyAuthorization { get }
```

## Discussion

If the value of this property is CLAccuracyAuthorization.fullAccuracy, you can set the desiredAccuracy property to any value. If the value is CLAccuracyAuthorization.reducedAccuracy, setting desiredAccuracy to a value other than kCLLocationAccuracyReduced has no effect on the location information, and your app can’t use region monitoring or beacon ranging.

Note

Because reduced accuracy isn’t available prior to watchOS 7, when the user chooses reduced accuracy on the paired iPhone, watch apps running with this older software don’t receive any location data. This occurs because watchOS apps must adhere to the permissions granted on the paired iPhone.

## See Also

### Determining the availability of services

class func significantLocationChangeMonitoringAvailable() -> Bool

Returns a Boolean value indicating whether the significant-change location service is available on the device.

class func headingAvailable() -> Bool

Returns a Boolean value indicating whether the location manager is able to generate heading-related events.

var isAuthorizedForWidgetUpdates: Bool

A Boolean value that indicates whether a widget is eligible to receive location updates.

class func isMonitoringAvailable(for: AnyClass) -> Bool

Returns a Boolean value indicating whether the device supports region monitoring using the specified class.

class func isRangingAvailable() -> Bool

Returns a Boolean value indicating whether the device supports ranging of beacons that use the iBeacon protocol.

class func locationServicesEnabled() -> Bool

Returns a Boolean value indicating whether location services are enabled on the device.

