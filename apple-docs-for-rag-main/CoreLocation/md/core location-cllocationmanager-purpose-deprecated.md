

- Core Location
- CLLocationManager
-  purpose Deprecated

Instance Property

# purpose

An app-provided string that describes the reason for using location services.

macOS 10.7–11.0Deprecated

``` source
var purpose: String? { get set }
```

Deprecated

Set the purpose string using the NSLocationWhenInUseUsageDescription key in the app’s `Info.plist` instead.

## Discussion

If this property isn’t `nil` and the system needs to ask for the user’s consent to use location services, it displays the provided string. You can use this string to explain why your app is using location services.

You must set the value of this property prior to starting any location services. Because the string is ultimately displayed to the user, you should always load it from a localized strings file.

## See Also

### Properties

var headingAvailable: Bool

A Boolean value indicating whether the location manager is able to generate heading-related events.

Deprecated

var locationServicesEnabled: Bool

A Boolean value indicating whether location services are enabled on the device.

Deprecated

var rangedRegions: Set&lt;CLRegion>

The set of regions currently being tracked using ranging.

Deprecated

