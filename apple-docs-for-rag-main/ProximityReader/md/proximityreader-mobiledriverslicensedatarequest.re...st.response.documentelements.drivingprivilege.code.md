

- ProximityReader
- MobileDriversLicenseDataRequest
- 
  - MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
- MobileDriversLicenseDataRequest.Response.DocumentElements
- MobileDriversLicenseDataRequest.Response.DocumentElements.DrivingPrivilege
-  MobileDriversLicenseDataRequest.Response.DocumentElements.DrivingPrivilege.Code 

Structure

# MobileDriversLicenseDataRequest.Response.DocumentElements.DrivingPrivilege.Code

An object representing a code of a driving privilege.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Code
```

## Topics

### Operators

static func == (MobileDriversLicenseDataRequest.Response.DocumentElements.DrivingPrivilege.Code, MobileDriversLicenseDataRequest.Response.DocumentElements.DrivingPrivilege.Code) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let code: String

The code of a driving privilege.

var hashValue: Int

The hash value.

let sign: String?

The sign of a driving privilege code.

let value: String?

The value of a driving privilege code.

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

