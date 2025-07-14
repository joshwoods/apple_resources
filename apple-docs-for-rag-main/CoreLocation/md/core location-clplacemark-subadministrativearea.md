

- Core Location
- CLPlacemark
-  subAdministrativeArea 

Instance Property

# subAdministrativeArea

Additional administrative area information for the placemark.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var subAdministrativeArea: String? { get }
```

## Discussion

Subadministrative areas typically correspond to counties or other regions that are then organized into a larger administrative area or state. For example, if the placemark location is Apple’s headquarters, the value for this property would be the string “Santa Clara”, which is the county in California that contains the city of Cupertino.

## See Also

### Getting the placemark details

var thoroughfare: String?

The street address associated with the placemark.

var subThoroughfare: String?

Additional street-level information for the placemark.

var locality: String?

The city associated with the placemark.

var subLocality: String?

Additional city-level information for the placemark.

var administrativeArea: String?

The state or province associated with the placemark.

var postalCode: String?

The postal code associated with the placemark.

