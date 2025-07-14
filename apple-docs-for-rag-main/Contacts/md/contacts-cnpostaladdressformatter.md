

- Contacts
-  CNPostalAddressFormatter 

Class

# CNPostalAddressFormatter

An object that you use to format a contact’s postal addresses.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNPostalAddressFormatter
```

## Overview

A `CNPostalAddressFormatter` object handles international formatting of postal addresses. It is recommended that you create an instance of this class when formatting many postal addresses, and use the instance methods; otherwise use the class methods.

## Topics

### Generating a formatted attributed string

func attributedString(from: CNPostalAddress, withDefaultAttributes: [AnyHashable : Any]) -> NSAttributedString

Returns a formatted postal address as an attributed string.

class func attributedString(from: CNPostalAddress, style: CNPostalAddressFormatterStyle, withDefaultAttributes: [AnyHashable : Any]) -> NSAttributedString

Returns a postal address as an attributed string and formatted for the specified style.

let CNPostalAddressPropertyAttribute: String

An attribute that identifies the purpose of a range of characters in an attributed string.

let CNPostalAddressLocalizedPropertyNameAttribute: String

An attribute that identifies the localized property of postal address.

### Generating a formatted string

func string(from: CNPostalAddress) -> String

Returns a formatted postal address.

class func string(from: CNPostalAddress, style: CNPostalAddressFormatterStyle) -> String

Returns a postal address as a string and formatted for the specified style.

### Specifying the formatting style

var style: CNPostalAddressFormatterStyle

The style to apply when formatting strings.

enum CNPostalAddressFormatterStyle

Constants for postal formatting styles.

### Getting the postal attribute keys

let CNPostalAddressCityKey: String

The city of the address.

let CNPostalAddressCountryKey: String

The country or region name of the address.

let CNPostalAddressISOCountryCodeKey: String

The ISO country code of the address.

let CNPostalAddressPostalCodeKey: String

The postal code of the address.

let CNPostalAddressStateKey: String

The state name of the address.

let CNPostalAddressStreetKey: String

The street name of the address.

let CNPostalAddressSubAdministrativeAreaKey: String

The subadministrative area of the address.

let CNPostalAddressSubLocalityKey: String

The sublocality of the address.

## Relationships

### Inherits From

- Formatter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Formatters

class CNContactFormatter

An object that you use to format contact information before displaying it to the user.

class CNContactVCardSerialization

An object you use to convert to and from a vCard representation of the user’s contacts.

class CNContactsUserDefaults

An object that defines the default options to use when displaying contacts.

