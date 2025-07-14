

- ProximityReader
- MobileNationalIDCardDisplayRequest
-  MobileNationalIDCardDisplayRequest.Element 

Structure

# MobileNationalIDCardDisplayRequest.Element

A type that represents an element you can request from a mobile national ID card.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct Element
```

## Topics

### Operators

static func == (MobileNationalIDCardDisplayRequest.Element, MobileNationalIDCardDisplayRequest.Element) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let age: MobileNationalIDCardDisplayRequest.Element

The mobile national ID card holder’s age in years.

static let familyName: MobileNationalIDCardDisplayRequest.Element

The mobile national ID card holder’s family name or last name.

static let givenName: MobileNationalIDCardDisplayRequest.Element

The mobile national ID card holder’s given name or first name.

### Type Methods

static func ageAtLeast(Int) -> MobileNationalIDCardDisplayRequest.Element

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

var elements: [MobileNationalIDCardDisplayRequest.Element]

The document elements you’re requesting.

var options: MobileNationalIDCardDisplayRequest.Options

An object that customizes how to perform a display request.

struct Options

An object that customizes how to perform a display request.

