

- ProximityReader
- MobileDriversLicenseRawDataRequest
-  MobileDriversLicenseRawDataRequest.Element 

Structure

# MobileDriversLicenseRawDataRequest.Element

A type representing an element that you can request from a mobile driver’s license.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Element
```

## Topics

### Operators

static func == (MobileDriversLicenseRawDataRequest.Element, MobileDriversLicenseRawDataRequest.Element) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let address: MobileDriversLicenseRawDataRequest.Element

The mobile driver’s license holder’s address on record with the issuer.

static let age: MobileDriversLicenseRawDataRequest.Element

The mobile driver’s license holder’s age in years.

static let dateOfBirth: MobileDriversLicenseRawDataRequest.Element

The date of birth of the mobile driver’s license holder.

static let documentDHSComplianceStatus: MobileDriversLicenseRawDataRequest.Element

The document’s DHS (U.S. Department of Homeland Security) compliance status.

static let documentExpirationDate: MobileDriversLicenseRawDataRequest.Element

The document’s expiration date.

static let documentIssueDate: MobileDriversLicenseRawDataRequest.Element

The document’s issue date.

static let documentNumber: MobileDriversLicenseRawDataRequest.Element

The document’s number, as defined by the document’s issuing authority.

static let drivingPrivileges: MobileDriversLicenseRawDataRequest.Element

The mobile driver’s license holder’s driving privileges.

static let familyName: MobileDriversLicenseRawDataRequest.Element

The mobile driver’s license holder’s family name or last name.

static let givenName: MobileDriversLicenseRawDataRequest.Element

The mobile driver’s license holder’s given name or first name.

static let issuingAuthority: MobileDriversLicenseRawDataRequest.Element

The state or government that issued the identity document.

static let portrait: MobileDriversLicenseRawDataRequest.Element

The portrait of the mobile driver’s license holder on record with the issuer.

static let sex: MobileDriversLicenseRawDataRequest.Element

The mobile driver’s license holder’s sex.

### Type Methods

static func ageAtLeast(Int) -> MobileDriversLicenseRawDataRequest.Element

A Boolean value that indicates whether the mobile driver’s license holder’s age is at least the given age.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Creating a raw data request

init(retainedElements: [MobileDriversLicenseRawDataRequest.Element], nonRetainedElements: [MobileDriversLicenseRawDataRequest.Element])

Returns a mobile driver’s license raw data request.

var retainedElements: [MobileDriversLicenseRawDataRequest.Element]

The document elements you’re requesting and intend to retain for an indefinite period of time.

var nonRetainedElements: [MobileDriversLicenseRawDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than is necessary to process the result in realtime.

