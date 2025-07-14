

- ProximityReader
- MobileDriversLicenseDisplayRequest
-  MobileDriversLicenseDisplayRequest.Element 

Structure

# MobileDriversLicenseDisplayRequest.Element

A type that represents an element you can request from a mobile driver’s license.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Element
```

## Topics

### Operators

static func == (MobileDriversLicenseDisplayRequest.Element, MobileDriversLicenseDisplayRequest.Element) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let age: MobileDriversLicenseDisplayRequest.Element

The mobile driver’s license holder’s age in years.

static let familyName: MobileDriversLicenseDisplayRequest.Element

The mobile driver’s license holder’s family name or last name.

static let givenName: MobileDriversLicenseDisplayRequest.Element

The mobile driver’s license holder’s given name or first name.

### Type Methods

static func ageAtLeast(Int) -> MobileDriversLicenseDisplayRequest.Element

A Boolean value that indicates whether the mobile driver’s license holder’s age is at least the given age.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Creating a display request

init(elements: [MobileDriversLicenseDisplayRequest.Element], options: MobileDriversLicenseDisplayRequest.Options)

Creates a new mobile driver’s license display request.

var elements: [MobileDriversLicenseDisplayRequest.Element]

The document elements you’re requesting.

