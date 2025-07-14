

- ProximityReader
- MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
- MobileDriversLicenseDataRequest.Response.DocumentElements
-  MobileDriversLicenseDataRequest.Response.DocumentElements.IssuingAuthority 

Structure

# MobileDriversLicenseDataRequest.Response.DocumentElements.IssuingAuthority

A type that represents the state or government that issued the identity document.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct IssuingAuthority
```

## Topics

### Operators

static func == (MobileDriversLicenseDataRequest.Response.DocumentElements.IssuingAuthority, MobileDriversLicenseDataRequest.Response.DocumentElements.IssuingAuthority) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let isoCountryCode: String?

The country that issued the identity document.

let jurisdiction: String?

The name of the jurisdiction that issued the identity document.

let name: String?

The name of the state or government that issued the identity document.

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

