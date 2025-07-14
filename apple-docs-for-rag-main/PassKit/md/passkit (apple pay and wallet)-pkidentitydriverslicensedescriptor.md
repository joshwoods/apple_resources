

- PassKit (Apple Pay and Wallet)
-  PKIdentityDriversLicenseDescriptor 

Class

# PKIdentityDriversLicenseDescriptor

An object for requesting information from a user’s driver’s license or equivalent document.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class PKIdentityDriversLicenseDescriptor
```

## Mentioned in 

Requesting identity data from a Wallet pass

## Overview

For the elements you request, the response contains the corresponding elements present in the user’s identity document. The table below maps the elements you request using PKIdentityElement with the ISO and American Association of Motor Vehicle Administrators (AAMVA) namespaces in the response.

Important

When you verify a person’s driving privileges from a U.S. driver’s license, use `domestic_driving_privileges` from the `org.iso.18013.5.1.aamva` namespace instead of `driving_privileges` from the `org.iso.18013.5.1` namespace because the former maps more directly to state laws. For more information about implementation, see AAMVA Mobile Driver’s License (mDL) Implementation Guidelines.

The framework allows for requesting the Boolean age(atLeast:) element for any age between `1` and `125` only if the issuer includes it. If an app requests age(atLeast:) and the `age_over_XX` element isn’t present in the mobile driver’s license, the framework falls back to a request for the age element.

An app can’t include both an age(atLeast:) element and an age element in the same request.

| Identity element | ISO namespace | AAMVA namespace |
|----|----|----|
| `givenName` | `given_name` | `given_name_truncation`, `aka_given_name`, `name_suffix`, `aka_suffix` |
| `familyName` | `family_name` | `family_name_truncation`, `aka_family_name` |
| `portrait` | `portrait` |  |
| `address` | `resident_address`, `resident_city`, `resident_country`, `resident_postal_code` |  |
| `issuingAuthority` | `issuing_authority`, `issuing_jurisdiction`, `issuing_country`, `un_distinguishing_sign` |  |
| `documentExpirationDate` | `expiry_date` |  |
| `documentIssueDate` | `document_issue_date` |  |
| `documentNumber` | `document_number` |  |
| `drivingPrivileges` | `driving_privileges` | `domestic_driving_privileges` |
| `age` | `age_in_years` |  |
| `dateOfBirth` | `birth_date` |  |
| `age(atLeast: XX)` | `age_over_XX` |  |

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- PKIdentityDocumentDescriptor

## See Also

### Describing a document

class PKIdentityIntentToStore

An object that represents your intention to store an identity element or values derived from an identity element.

protocol PKIdentityDocumentDescriptor

A type that describes the structure and behavior of an identity document.

