

- ProximityReader
- MobileNationalIDCardDataRequest
-  MobileNationalIDCardDataRequest.Element 

Structure

# MobileNationalIDCardDataRequest.Element

A type that represents an element you can request from a mobile national ID card.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct Element
```

## Topics

### Operators

static func == (MobileNationalIDCardDataRequest.Element, MobileNationalIDCardDataRequest.Element) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let age: MobileNationalIDCardDataRequest.Element

The mobile national ID card holder’s age in years.

static let dateOfBirth: MobileNationalIDCardDataRequest.Element

The date of birth of the mobile national ID card holder.

static let documentNumber: MobileNationalIDCardDataRequest.Element

The document’s number, as defined by the document’s issuing authority.

static let familyName: MobileNationalIDCardDataRequest.Element

The mobile national ID card holder’s family name or last name.

static let givenName: MobileNationalIDCardDataRequest.Element

The mobile national ID card holder’s given name or first name.

static let portrait: MobileNationalIDCardDataRequest.Element

The picture of the mobile national ID card holder on record with the issuer.

static let sex: MobileNationalIDCardDataRequest.Element

The mobile national ID card holder’s sex.

### Type Methods

static func ageAtLeast(Int) -> MobileNationalIDCardDataRequest.Element

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

var retainedElements: [MobileNationalIDCardDataRequest.Element]

The document elements you’re requesting and intend to retain for an indefinite period of time.

var nonRetainedElements: [MobileNationalIDCardDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than necessary to process the result in realtime.

