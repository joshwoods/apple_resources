

- ARKit
- ARGeoTrackingConfiguration
-  checkAvailability(at:completionHandler:) 

Type Method

# checkAvailability(at:completionHandler:)

Determines if geotracking supports a particular location.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class func checkAvailability(
    at coordinate: CLLocationCoordinate2D,
    completionHandler: @escaping (Bool, (any Error)?) -> Void
)
```

## Parameters 

`coordinate`  

The GPS location that the framework checks for availability.

`completionHandler`  

Code you supply that runs after the function returns. The closure takes a Boolean argument that indicates whether geotracking is available.

## Discussion

This function returns false under the following circumstances:

- ARKit lacks localization imagery for the argument GPS coordinate.

- A network connection is unavailable to download localization imagery.

- The device lacks cellular (GPS) capability.

To determine availability at the user’s GPS coordinate, use checkAvailability(completionHandler:) instead.

For a list of supported areas and cities, see ARGeoTrackingConfiguration.

## See Also

### Checking Availability

class func checkAvailability(completionHandler: (Bool, (any Error)?) -> Void)

Determines if geotracking supports the user’s current location.

