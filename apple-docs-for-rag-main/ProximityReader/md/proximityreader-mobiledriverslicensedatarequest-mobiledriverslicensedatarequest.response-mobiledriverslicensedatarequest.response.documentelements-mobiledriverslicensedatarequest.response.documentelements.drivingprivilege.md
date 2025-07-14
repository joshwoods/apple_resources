

- ProximityReader
- MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
- MobileDriversLicenseDataRequest.Response.DocumentElements
-  MobileDriversLicenseDataRequest.Response.DocumentElements.DrivingPrivilege 

Structure

# MobileDriversLicenseDataRequest.Response.DocumentElements.DrivingPrivilege

A type that represents a driving privilege which the mobile driver’s license holder possesses.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct DrivingPrivilege
```

## Topics

### Structures

struct Code

An object representing a code of a driving privilege.

### Operators

static func == (MobileDriversLicenseDataRequest.Response.DocumentElements.DrivingPrivilege, MobileDriversLicenseDataRequest.Response.DocumentElements.DrivingPrivilege) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let codes: [MobileDriversLicenseDataRequest.Response.DocumentElements.DrivingPrivilege.Code]

The codes which describe the driving privilege.

let expirationDate: DateComponents?

The expiration date of the driving privilege.

var hashValue: Int

The hash value.

let issueDate: DateComponents?

The issue date of the driving privilege.

let vehicleCategoryCode: String

The vehicle category code of the driving privilege.

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

