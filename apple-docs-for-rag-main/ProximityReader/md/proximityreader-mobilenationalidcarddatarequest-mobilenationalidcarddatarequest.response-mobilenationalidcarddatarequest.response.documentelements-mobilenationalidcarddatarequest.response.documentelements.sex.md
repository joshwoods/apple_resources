

- ProximityReader
- MobileNationalIDCardDataRequest
- MobileNationalIDCardDataRequest.Response
- MobileNationalIDCardDataRequest.Response.DocumentElements
-  MobileNationalIDCardDataRequest.Response.DocumentElements.Sex 

Enumeration

# MobileNationalIDCardDataRequest.Response.DocumentElements.Sex

A type that represents the mobile national ID card holder’s sex.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
enum Sex
```

## Topics

### Operators

static func == (MobileNationalIDCardDataRequest.Response.DocumentElements.Sex, MobileNationalIDCardDataRequest.Response.DocumentElements.Sex) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case female

A constant that indicates the mobile national ID card holder is female as defined in ISO/IEC 5218.

case male

A constant that indicates the mobile national ID card holder is male as defined in ISO/IEC 5218.

case notApplicable

A constant that indicates the mobile national ID card holder’s sex was categorized as not applicable as defined in ISO/IEC 5218.

case unknown

A constant that indicates the mobile national ID card holder’s sex is not known as defined in ISO/IEC 5218.

### Instance Properties

var hashValue: Int

The hash value.

var localizedName: String

A string containing the the localized name of the sex category.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

