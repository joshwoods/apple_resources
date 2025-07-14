

- ProximityReader
- MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
-  MobileDriversLicenseDataRequest.Response.DocumentElements 

Structure

# MobileDriversLicenseDataRequest.Response.DocumentElements

A type that contains the document elements from a successful mobile driver’s license data request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct DocumentElements
```

## Topics

### Structures

struct AAMVADrivingPrivilege

A type that represents the mobile driver’s license holder’s AAMVA driving privileges.

struct DrivingPrivilege

A type that represents a driving privilege which the mobile driver’s license holder possesses.

struct IssuingAuthority

A type that represents the state or government that issued the identity document.

### Operators

static func == (MobileDriversLicenseDataRequest.Response.DocumentElements, MobileDriversLicenseDataRequest.Response.DocumentElements) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let aamvaDrivingPrivileges: [MobileDriversLicenseDataRequest.Response.DocumentElements.AAMVADrivingPrivilege]

The mobile driver’s license holder’s AAMVA driving privileges.

var address: CNPostalAddress?

The mobile driver’s license holder’s address on record with the issuer.

let age: Int?

The mobile driver’s license holder’s age in years.

let ageAtLeastElements: [Int : Bool]

A dictionary of values that indicate whether the document holder is at least the specified age.

let dateOfBirth: DateComponents?

The date of birth of the mobile driver’s license holder.

let documentDHSComplianceStatus: MobileDriversLicenseDataRequest.Response.DocumentElements.DHSComplianceStatus?

The document’s DHS (U.S. Department of Homeland Security) compliance status.

let documentExpirationDate: DateComponents?

The document’s expiration date.

let documentIssueDate: DateComponents?

The document’s issue date.

let documentNumber: String?

The document’s number, as defined by the document’s issuing authority.

let drivingPrivileges: [MobileDriversLicenseDataRequest.Response.DocumentElements.DrivingPrivilege]

The mobile driver’s license holder’s driving privileges.

var hashValue: Int

The hash value.

let issuingAuthority: MobileDriversLicenseDataRequest.Response.DocumentElements.IssuingAuthority?

The state or government that issued the identity document.

let nameComponents: PersonNameComponents?

The mobile driver’s license holder’s name components.

let portraitData: Data?

The portrait data of the mobile driver’s license holder on record with the issuer.

let sex: MobileDriversLicenseDataRequest.Response.DocumentElements.Sex?

The mobile driver’s license holder’s sex.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum DHSComplianceStatus

A type that represents the mobile driver’s license’ DHS (U.S. Department of Homeland Security) compliance status.

enum Sex

A type that represents the mobile driver’s license holder’s sex.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

