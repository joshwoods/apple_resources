

- UIKit
-  UITextContentType 

Structure

# UITextContentType

Constants that identify the semantic meaning for a text-entry area.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct UITextContentType
```

## Overview

Use these constants with the textContentType property.

## Topics

### Defining web addresses

static let URL: UITextContentType

A property that defines the content in a text input area as a URL.

### Identifying contacts

static let namePrefix: UITextContentType

A property that defines the content in a text input area as a prefix or title, such as *Dr*.

static let name: UITextContentType

A property that defines the content in a text input area as a name.

static let nameSuffix: UITextContentType

A property that defines the content in a text input area as a suffix, such as *Jr*.

static let givenName: UITextContentType

A property that defines the content in a text input area as a first name.

static let middleName: UITextContentType

A property that defines the content in a text input area as a middle name.

static let familyName: UITextContentType

A property that defines the content in a text input area as a family name, or last name.

static let nickname: UITextContentType

A property that defines the content in a text input area as a nickname.

static let organizationName: UITextContentType

A property that defines the content in a text input area as an organization name.

static let jobTitle: UITextContentType

A property that defines the content in a text input area as a job title.

### Setting location data

static let location: UITextContentType

A property that defines the content in a text input area as a location, such as a point of interest, an address, or another identifier for a location.

static let fullStreetAddress: UITextContentType

A property that defines the content in a text input area as a street address that fully identifies a location.

static let streetAddressLine1: UITextContentType

A property that defines the content in a text input area as the first line of a street address.

static let streetAddressLine2: UITextContentType

A property that defines the content in a text input area as the second line of a street address.

static let addressCity: UITextContentType

A property that defines the content in a text input area as a city name.

static let addressCityAndState: UITextContentType

A property that defines the content in a text input area as a city name with a state name.

static let addressState: UITextContentType

A property that defines the content in a text input area as a state name.

static let postalCode: UITextContentType

A property that defines the content in a text input area as a postal code.

static let sublocality: UITextContentType

A property that defines the content in a text input area as a sublocality.

static let countryName: UITextContentType

A property that defines the content in a text input area as a country or region name.

### Managing accounts

static let username: UITextContentType

A property that defines the content in a text input area as an account or login name.

static let password: UITextContentType

A property that defines the content in a text input area as a password.

static let newPassword: UITextContentType

A property that defines the content in a text input area as a new password.

### Securing accounts

static let oneTimeCode: UITextContentType

A property that defines the content in a text input area as a one-time code.

### Setting communication details

static let emailAddress: UITextContentType

A property that defines the content in a text input area as an email address.

static let telephoneNumber: UITextContentType

A property that defines the content in a text input area as a telephone number.

static let cellularEID: UITextContentType

A property that defines the content in a text input area to contain an embedded identity document number for an eSIM.

static let cellularIMEI: UITextContentType

A property that defines the content in a text input area to contain an international mobile equipment identity number for an eSIM.

### Accepting payment

static let creditCardNumber: UITextContentType

A property that defines the content in a text input area as a credit card number.

static let creditCardExpiration: UITextContentType

A property that defines the content in a text input area as an expiration date on a credit card.

static let creditCardExpirationMonth: UITextContentType

A property that defines the content in a text input area as the month component of an expiration date on a credit card.

static let creditCardExpirationYear: UITextContentType

A property that defines the content in a text input area as the year component of an expiration date on a credit card.

static let creditCardSecurityCode: UITextContentType

A property that defines the content in a text input area as a credit card security code.

static let creditCardType: UITextContentType

A property that defines the content in a text input area as a credit card type.

static let creditCardName: UITextContentType

A property that defines the content in a text input area as a name on a credit card.

static let creditCardGivenName: UITextContentType

A property that defines the content in a text input area as a first name on a credit card.

static let creditCardMiddleName: UITextContentType

A property that defines the content in a text input area as a middle name on a credit card.

static let creditCardFamilyName: UITextContentType

A property that defines the content in a text input area as a family name, or last name, on a credit card.

### Getting birthday information

static let birthdate: UITextContentType

A property that defines the content in a text input area as a date of birth.

static let birthdateDay: UITextContentType

A property that defines the content in a text input area as the day component of a birthdate.

static let birthdateMonth: UITextContentType

A property that defines the content in a text input area as the month component of a birthdate.

static let birthdateYear: UITextContentType

A property that defines the content in a text input area as the year component of a birthdate.

### Scheduling events

static let dateTime: UITextContentType

A property that defines the content in a text input area as a date, time, or duration.

### Tracking events

static let flightNumber: UITextContentType

A property that defines the content in a text input area as an airline flight number.

static let shipmentTrackingNumber: UITextContentType

A property that defines the content in a text input area as a parcel tracking number.

### Creating a text content type

init(rawValue: String)

Creates a text content type with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the keyboard appearance

var keyboardType: UIKeyboardType

The keyboard type for the text object.

enum UIKeyboardType

Constants that specify the type of keyboard to display for a text-based view.

var keyboardAppearance: UIKeyboardAppearance

The appearance style of the keyboard for the text object.

enum UIKeyboardAppearance

Constants that specify the appearance of the keyboard for a text-based view.

var returnKeyType: UIReturnKeyType

The visible title of the Return key.

enum UIReturnKeyType

Constants that specify the text string that displays in the Return key of a keyboard.

var textContentType: UITextContentType!

The semantic meaning for a text input area.

