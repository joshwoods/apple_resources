

- WatchKit
-  WKTextContentType 

Structure

# WKTextContentType

Constants that specify a text field’s semantic meaning.

watchOS

``` source
struct WKTextContentType
```

## Topics

### Name

static let name: WKTextContentType

A full name.

static let namePrefix: WKTextContentType

A title or prefix for a name.

static let givenName: WKTextContentType

A given name.

static let middleName: WKTextContentType

A middle name.

static let familyName: WKTextContentType

A last name.

static let nameSuffix: WKTextContentType

A suffix for a name.

static let nickname: WKTextContentType

A nickname.

### Employment

static let jobTitle: WKTextContentType

A job title.

static let organizationName: WKTextContentType

An organization’s name.

### Address

static let location: WKTextContentType

A point of interest, address, or other identifiable location.

static let fullStreetAddress: WKTextContentType

The full street address for a location, including the unit or suite number.

static let streetAddressLine1: WKTextContentType

The first line of a street address.

static let streetAddressLine2: WKTextContentType

The second line of a street address.

static let addressCity: WKTextContentType

The name of a city.

static let addressState: WKTextContentType

The name of a state.

static let addressCityAndState: WKTextContentType

The name of a city and state.

static let sublocality: WKTextContentType

The sublocality.

static let countryName: WKTextContentType

The name of a country or region.

static let postalCode: WKTextContentType

A postal code.

### Contact Information

static let telephoneNumber: WKTextContentType

A telephone number.

static let emailAddress: WKTextContentType

An email address.

### Other

static let URL: WKTextContentType

A URL.

static let creditCardNumber: WKTextContentType

A credit card number.

### Login Credentials

static let username: WKTextContentType

An account or login name.

static let password: WKTextContentType

An existing password.

static let newPassword: WKTextContentType

A new password.

static let oneTimeCode: WKTextContentType

A one-time code.

### Initializers

init(rawValue: String)

Returns a newly instantiated content type.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the Content Type

func setTextContentType(WKTextContentType?)

Sets the text field’s semantic meaning.

