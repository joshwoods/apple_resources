

- ProximityReader
- MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
- MobileDriversLicenseDataRequest.Response.DocumentElements
-  MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege 

Structure

# MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege

A type that represents the mobile driver’s license holder’s AAMVA driving privileges.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct AAMVADrivingPrivilege
```

## Topics

### Structures

struct VehicleClass

An object that represents the driving privilege vehicle class.

struct VehicleEndorsement

An object that represents an endorsement on a driving privilege.

struct VehicleRestriction

An object that represents a restriction on a driving privilege.

### Operators

static func == (MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege, MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let vehicleClass: MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleClass?

The driving privilege vehicle class.

let vehicleEndorsements: [MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleEndorsement]

The endorsements on the driving privilege.

let vehicleRestrictions: [MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleRestriction]

The restrictions on the driving privilege.

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

