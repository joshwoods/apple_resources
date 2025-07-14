

- ProximityReader
- MobileDriversLicenseDataRequest
- 
  - MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
- MobileDriversLicenseDataRequest.Response.DocumentElements
- MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege
-  MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleClass 

Structure

# MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleClass

An object that represents the driving privilege vehicle class.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct VehicleClass
```

## Topics

### Operators

static func == (MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleClass, MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege.VehicleClass) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let code: String

The code of the vehicle class privilege.

let description: String

The description of the vehicle class privilege.

let expirationDate: DateComponents?

The expiration date of the vehicle class privilege.

var hashValue: Int

The hash value.

let issueDate: DateComponents?

The issue date of the vehicle class privilege.

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

