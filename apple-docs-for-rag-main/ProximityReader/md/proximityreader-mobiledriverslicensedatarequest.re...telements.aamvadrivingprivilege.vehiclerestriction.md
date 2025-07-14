

- ProximityReader
- MobileDriversLicenseDataRequest
- 
  - MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
- MobileDriversLicenseDataRequest.Response.DocumentElements
- MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege
-  MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleRestriction 

Structure

# MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleRestriction

An object that represents a restriction on a driving privilege.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct VehicleRestriction
```

## Topics

### Operators

static func == (MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleRestriction, MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleRestriction) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let code: String?

The code of the vehicle restriction.

let description: String

The description of the vehicle restriction.

var hashValue: Int

The hash value.

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

