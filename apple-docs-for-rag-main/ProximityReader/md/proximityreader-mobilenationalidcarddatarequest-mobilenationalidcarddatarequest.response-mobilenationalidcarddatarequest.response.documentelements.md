

- ProximityReader
- MobileNationalIDCardDataRequest
- MobileNationalIDCardDataRequest.Response
-  MobileNationalIDCardDataRequest.Response.DocumentElements 

Structure

# MobileNationalIDCardDataRequest.Response.DocumentElements

A type that contains the document elements from a successful mobile national ID card data request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct DocumentElements
```

## Topics

### Operators

static func == (MobileNationalIDCardDataRequest.Response.DocumentElements, MobileNationalIDCardDataRequest.Response.DocumentElements) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let age: Int?

The mobile national ID card holder’s age in years.

let ageAtLeastElements: [Int : Bool]

A dictionary of values that indicate whether the document holder is at least the specified age.

let dateOfBirth: DateComponents?

The date of birth of the mobile national ID card holder.

let documentNumber: String?

The document’s number, as defined by the document’s issuing authority.

var hashValue: Int

The hash value.

let nameComponents: PersonNameComponents?

The mobile national ID card holder’s name components.

let portraitData: Data?

The portrait data of the mobile national ID card holder on record with the issuer.

let sex: MobileNationalIDCardDataRequest.Response.DocumentElements.Sex?

The mobile national ID card holder’s sex.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum Sex

A type that represents the mobile national ID card holder’s sex.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

