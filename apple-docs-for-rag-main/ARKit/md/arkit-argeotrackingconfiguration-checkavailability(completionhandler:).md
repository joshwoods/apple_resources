

- ARKit
- ARGeoTrackingConfiguration
-  checkAvailability(completionHandler:) 

Type Method

# checkAvailability(completionHandler:)

Determines if geotracking supports the user’s current location.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class func checkAvailability(completionHandler: @escaping (Bool, (any Error)?) -> Void)
```

## Parameters 

`completionHandler`  

Code you supply that runs after the function returns. The closure takes a Boolean argument that indicates whether geotracking is available.

## Discussion

This function returns false under the following circumstances:

- ARKit lacks localization imagery for the user’s geographic position.

- A network connection is unavailable to download localization imagery.

- The device lacks cellular (GPS) capability.

To determine availability at a different location than the device’s current location, call checkAvailability(at:completionHandler:) instead.

For a list of supported areas and cities, see ARGeoTrackingConfiguration.

## See Also

### Checking Availability

class func checkAvailability(at: CLLocationCoordinate2D, completionHandler: (Bool, (any Error)?) -> Void)

Determines if geotracking supports a particular location.

