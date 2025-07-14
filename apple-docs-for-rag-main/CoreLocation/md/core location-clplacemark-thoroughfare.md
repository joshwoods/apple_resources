

- Core Location
- CLPlacemark
-  thoroughfare 

Instance Property

# thoroughfare

The street address associated with the placemark.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var thoroughfare: String? { get }
```

## Discussion

The street address contains the street name. For example, if the placemark location is Apple’s headquarters, the value for this property would be the string “Apple Park Way”.

## See Also

### Getting the placemark details

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

var postalCode: String?

The postal code associated with the placemark.

