

- Contacts
- CNPostalAddress
-  street 

Instance Property

# street

The street name in a postal address.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var street: String { get }
```

## Discussion

Multiline addresses are delimited by carriage returns (that is, “\n”).

## See Also

### Getting the Parts of a Postal Address

var city: String

The city name in a postal address.

var state: String

The state name in a postal address.

var postalCode: String

The postal code in a postal address.

var country: String

The country or region name in a postal address.

var isoCountryCode: String

The ISO country code for the country or region in a postal address, using the ISO 3166-1 alpha-2 standard.

var subAdministrativeArea: String

The subadministrative area (such as a county or other region) in a postal address.

var subLocality: String

Additional information associated with the location, typically defined at the city or town level, in a postal address.

