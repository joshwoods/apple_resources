

- Core Location
- CLPlacemark
-  subLocality 

Instance Property

# subLocality

Additional city-level information for the placemark.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var subLocality: String? { get }
```

## Discussion

This property contains additional information, such as the name of the neighborhood or landmark associated with the placemark. It might also refer to a common name that’s associated with the location.

## See Also

### Getting the placemark details

var thoroughfare: String?

The street address associated with the placemark.

var subThoroughfare: String?

Additional street-level information for the placemark.

var locality: String?

The city associated with the placemark.

var administrativeArea: String?

The state or province associated with the placemark.

var subAdministrativeArea: String?

Additional administrative area information for the placemark.

var postalCode: String?

The postal code associated with the placemark.

