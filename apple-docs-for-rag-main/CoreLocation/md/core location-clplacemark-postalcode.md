

- Core Location
- CLPlacemark
-  postalCode 

Instance Property

# postalCode

The postal code associated with the placemark.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var postalCode: String? { get }
```

## Discussion

If the placemark location is Apple’s headquarters, for example, the value for this property would be the string “95014”.

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

var subAdministrativeArea: String?

Additional administrative area information for the placemark.

