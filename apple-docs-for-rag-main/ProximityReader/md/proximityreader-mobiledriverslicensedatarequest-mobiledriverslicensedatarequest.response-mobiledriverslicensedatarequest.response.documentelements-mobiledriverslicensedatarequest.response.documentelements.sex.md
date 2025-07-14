

- ProximityReader
- MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
- MobileDriversLicenseDataRequest.Response.DocumentElements
-  MobileDriversLicenseDataRequest.Response.DocumentElements.Sex 

Enumeration

# MobileDriversLicenseDataRequest.Response.DocumentElements.Sex

A type that represents the mobile driver’s license holder’s sex.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+

``` source
enum Sex
```

## Topics

### Operators

static func == (MobileDriversLicenseDataRequest.Response.DocumentElements.Sex, MobileDriversLicenseDataRequest.Response.DocumentElements.Sex) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case female

A constant that indicates the mobile driver’s license holder is female as defined in ISO/IEC 5218.

case male

A constant that indicates the mobile driver’s license holder is male as defined in ISO/IEC 5218.

case notApplicable

A constant that indicates the mobile driver’s license holder’s sex was categorized as not applicable as defined in ISO/IEC 5218.

case notSpecified

A constant that indicates the mobile driver’s license holder’s sex was categorized as not specified or non-binary.

case unknown

A constant that indicates the mobile driver’s license holder’s sex is not known as defined in ISO/IEC 5218.

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

