

- ProximityReader
- MobileDriversLicenseDataRequest
-  MobileDriversLicenseDataRequest.Element 

Structure

# MobileDriversLicenseDataRequest.Element

A type that represents an element you can request from a mobile driver’s license.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Element
```

## Topics

### Operators

static func == (MobileDriversLicenseDataRequest.Element, MobileDriversLicenseDataRequest.Element) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let address: MobileDriversLicenseDataRequest.Element

The mobile driver’s license holder’s address on record with the issuer.

static let age: MobileDriversLicenseDataRequest.Element

The mobile driver’s license holder’s age in years.

static let dateOfBirth: MobileDriversLicenseDataRequest.Element

The date of birth of the mobile driver’s license holder.

static let documentDHSComplianceStatus: MobileDriversLicenseDataRequest.Element

The document’s DHS (U.S. Department of Homeland Security) compliance status.

static let documentExpirationDate: MobileDriversLicenseDataRequest.Element

The document’s expiration date.

static let documentIssueDate: MobileDriversLicenseDataRequest.Element

The document’s issue date.

static let documentNumber: MobileDriversLicenseDataRequest.Element

The document’s number, as defined by the document’s issuing authority.

static let drivingPrivileges: MobileDriversLicenseDataRequest.Element

The mobile driver’s license holder’s driving privileges.

static let familyName: MobileDriversLicenseDataRequest.Element

The mobile driver’s license holder’s family name or last name.

static let givenName: MobileDriversLicenseDataRequest.Element

The mobile driver’s license holder’s given name or first name.

static let issuingAuthority: MobileDriversLicenseDataRequest.Element

The state or government that issued the identity document.

static let portrait: MobileDriversLicenseDataRequest.Element

The picture of the mobile driver’s license holder on record with the issuer.

static let sex: MobileDriversLicenseDataRequest.Element

The mobile driver’s license holder’s sex.

### Type Methods

static func ageAtLeast(Int) -> MobileDriversLicenseDataRequest.Element

A Boolean value that indicates whether the mobile driver’s license holder’s age is at least the given age.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Creating a data request

init(retainedElements: [MobileDriversLicenseDataRequest.Element], nonRetainedElements: [MobileDriversLicenseDataRequest.Element])

Returns a mobile driver’s license data request.

var retainedElements: [MobileDriversLicenseDataRequest.Element]

The document elements you’re requesting and intend to retain for an indefinite period of time.

var nonRetainedElements: [MobileDriversLicenseDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than necessary to process the result in realtime.

