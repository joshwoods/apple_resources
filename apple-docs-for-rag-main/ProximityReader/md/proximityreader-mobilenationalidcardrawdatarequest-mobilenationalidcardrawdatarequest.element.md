

- ProximityReader
- MobileNationalIDCardRawDataRequest
-  MobileNationalIDCardRawDataRequest.Element 

Structure

# MobileNationalIDCardRawDataRequest.Element

A type representing an element that you can request from a mobile national ID card.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct Element
```

## Topics

### Operators

static func == (MobileNationalIDCardRawDataRequest.Element, MobileNationalIDCardRawDataRequest.Element) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let address: MobileNationalIDCardRawDataRequest.Element

The mobile national ID card holder’s address on record with the issuer.

static let age: MobileNationalIDCardRawDataRequest.Element

The mobile national ID card holder’s age in years.

static let dateOfBirth: MobileNationalIDCardRawDataRequest.Element

The date of birth of the mobile national ID card holder.

static let documentNumber: MobileNationalIDCardRawDataRequest.Element

The document’s number, as defined by the document’s issuing authority.

static let familyName: MobileNationalIDCardRawDataRequest.Element

The mobile national ID card holder’s family name or last name.

static let givenName: MobileNationalIDCardRawDataRequest.Element

The mobile national ID card holder’s given name or first name.

static let portrait: MobileNationalIDCardRawDataRequest.Element

The portrait of the mobile national ID card holder on record with the issuer.

static let sex: MobileNationalIDCardRawDataRequest.Element

The mobile national ID card holder’s sex.

### Type Methods

static func ageAtLeast(Int) -> MobileNationalIDCardRawDataRequest.Element

A Boolean value that indicates whether the mobile national ID card holder’s age is at least the given age.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Configuring the request details

var region: Locale.Region

The region of the document you’re requesting.

var retainedElements: [MobileNationalIDCardRawDataRequest.Element]

The document elements you’re requesting and intend to retain for an indefinite period of time.

var nonRetainedElements: [MobileNationalIDCardRawDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than is necessary to process the result in realtime.

