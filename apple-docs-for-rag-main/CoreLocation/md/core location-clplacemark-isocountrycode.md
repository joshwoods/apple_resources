

- Core Location
- CLPlacemark
-  isoCountryCode 

Instance Property

# isoCountryCode

The abbreviated country or region name.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isoCountryCode: String? { get }
```

## Discussion

This string is the standard abbreviation used to refer to the country or region. For example, if the placemark location is Apple’s headquarters, the value for this property would be the string “US”.

## See Also

### Getting the placemark’s country

var country: String?

The name of the country or region associated with the placemark.

