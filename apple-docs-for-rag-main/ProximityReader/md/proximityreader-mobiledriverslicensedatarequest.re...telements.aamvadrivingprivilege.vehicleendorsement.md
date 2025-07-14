

- ProximityReader
- MobileDriversLicenseDataRequest
- 
  - MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
- MobileDriversLicenseDataRequest.Response.DocumentElements
- MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege
-  MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleEndorsement 

Structure

# MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleEndorsement

An object that represents an endorsement on a driving privilege.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct VehicleEndorsement
```

## Topics

### Operators

static func == (MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleEndorsement, MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleEndorsement) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let code: String?

The code of the vehicle endorsement.

let description: String

The description of the vehicle endorsement.

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

