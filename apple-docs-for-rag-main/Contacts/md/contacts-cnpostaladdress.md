

- Contacts
-  CNPostalAddress 

Class

# CNPostalAddress

An immutable representation of the postal address for a contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNPostalAddress
```

## Overview

`CNPostalAddress` is a thread-safe class.

## Topics

### Getting the Parts of a Postal Address

var street: String

The street name in a postal address.

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

### Getting Localized Postal Values

class func localizedString(forKey: String) -> String

Returns the localized name for the property associated with the specified key.

let CNPostalAddressStreetKey: String

The street name of the address.

let CNPostalAddressCityKey: String

The city of the address.

let CNPostalAddressStateKey: String

The state name of the address.

let CNPostalAddressPostalCodeKey: String

The postal code of the address.

let CNPostalAddressCountryKey: String

The country or region name of the address.

let CNPostalAddressISOCountryCodeKey: String

The ISO country code of the address.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CNMutablePostalAddress

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Addresses

class CNMutablePostalAddress

A mutable representation of the postal address for a contact.

class CNInstantMessageAddress

An immutable object representing an instant message address for the contact.

