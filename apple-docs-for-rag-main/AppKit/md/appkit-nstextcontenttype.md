

- AppKit
-  NSTextContentType 

Structure

# NSTextContentType

Constants that identify the semantic meaning for a text-entry area.

macOS

``` source
struct NSTextContentType
```

## Discussion

Use these constants with the contentType property.

## Topics

### Creating a content type

init(rawValue: String)

Creates a new content type with the raw value you provide.

### Defining web addresses

static let URL: NSTextContentType

A property that defines the content in a text input area as a URL.

### Identifying contacts

static let namePrefix: NSTextContentType

A property that defines the content in a text input area as a prefix or title, such as *Dr*.

static let name: NSTextContentType

A property that defines the content in a text input area as a name.

static let nameSuffix: NSTextContentType

A property that defines the content in a text input area as a suffix, such as *Jr*.

static let givenName: NSTextContentType

A property that defines the content in a text input area as a first name.

static let middleName: NSTextContentType

A property that defines the content in a text input area as a middle name.

static let familyName: NSTextContentType

A property that defines the content in a text input area as a family name, or last name.

static let nickname: NSTextContentType

A property that defines the content in a text input area as a nickname.

static let organizationName: NSTextContentType

A property that defines the content in a text input area as an organization name.

static let jobTitle: NSTextContentType

A property that defines the content in a text input area as a job title.

### Setting location data

static let location: NSTextContentType

A property that defines the content in a text input area as a location, such as a point of interest, an address, or another identifier for a location.

static let fullStreetAddress: NSTextContentType

A property that defines the content in a text input area as a street address that fully identifies a location.

static let streetAddressLine1: NSTextContentType

A property that defines the content in a text input area as the first line of a street address.

static let streetAddressLine2: NSTextContentType

A property that defines the content in a text input area as the second line of a street address.

static let addressCity: NSTextContentType

A property that defines the content in a text input area as a city name.

static let addressCityAndState: NSTextContentType

A property that defines the content in a text input area as a city name with a state name.

static let addressState: NSTextContentType

A property that defines the content in a text input area as a state name.

static let postalCode: NSTextContentType

A property that defines the content in a text input area as a postal code.

static let sublocality: NSTextContentType

A property that defines the content in a text input area as a sublocality.

static let countryName: NSTextContentType

A property that defines the content in a text input area as a country or region name.

### Managing accounts

static let username: NSTextContentType

A property that defines the content in a text input area as an account or login name.

static let password: NSTextContentType

A property that defines the content in a text input area as a password.

static let newPassword: NSTextContentType

A property that defines the content in a text input area as a new password.

### Securing accounts

static let oneTimeCode: NSTextContentType

A property that defines the content in a text input area as a one-time code.

### Setting communication details

static let emailAddress: NSTextContentType

A property that defines the content in a text input area as an email address.

static let telephoneNumber: NSTextContentType

A property that defines the content in a text input area as a telephone number.

### Accepting payment

static let creditCardNumber: NSTextContentType

A property that defines the content in a text input area as a credit card number.

static let creditCardExpiration: NSTextContentType

A property that defines the content in a text input area as an expiration date on a credit card.

static let creditCardExpirationMonth: NSTextContentType

A property that defines the content in a text input area as the month component of an expiration date on a credit card.

static let creditCardExpirationYear: NSTextContentType

A property that defines the content in a text input area as the year component of an expiration date on a credit card.

static let creditCardSecurityCode: NSTextContentType

A property that defines the content in a text input area as a credit card security code.

static let creditCardType: NSTextContentType

A property that defines the content in a text input area as a credit card type.

static let creditCardName: NSTextContentType

A property that defines the content in a text input area as a name on a credit card.

static let creditCardGivenName: NSTextContentType

A property that defines the content in a text input area as a first name on a credit card.

static let creditCardMiddleName: NSTextContentType

A property that defines the content in a text input area as a middle name on a credit card.

static let creditCardFamilyName: NSTextContentType

A property that defines the content in a text input area as a family name, or last name, on a credit card.

### Getting birthday information

static let birthdate: NSTextContentType

A property that defines the content in a text input area as a date of birth.

static let birthdateDay: NSTextContentType

A property that defines the content in a text input area as the day component of a birthdate.

static let birthdateMonth: NSTextContentType

A property that defines the content in a text input area as the month component of a birthdate.

static let birthdateYear: NSTextContentType

A property that defines the content in a text input area as the year component of a birthdate.

### Scheduling events

static let dateTime: NSTextContentType

A property that defines the content in a text input area as a date, time, or duration.

### Tracking events

static let flightNumber: NSTextContentType

A property that defines the content in a text input area as an airline flight number.

static let shipmentTrackingNumber: NSTextContentType

A property that defines the content in a text input area as a parcel tracking number.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying content type

var contentType: NSTextContentType?

The semantic meaning for a text input area.

**Required**

