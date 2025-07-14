

- MapKit
- MKUserLocation
-  heading 

Instance Property

# heading

The heading of the user’s location.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.9+

``` source
var heading: CLHeading? { get }
```

## Discussion

This property is `nil` if the user’s location tracking mode isn’t MKUserTrackingMode.followWithHeading.

## See Also

### Determining the user’s location

var location: CLLocation?

The location of the device.

var isUpdating: Bool

A Boolean value that indicates whether the map view is updating the user’s location.

