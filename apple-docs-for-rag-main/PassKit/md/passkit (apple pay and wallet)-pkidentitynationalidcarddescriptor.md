

- PassKit (Apple Pay and Wallet)
-  PKIdentityNationalIDCardDescriptor 

Class

# PKIdentityNationalIDCardDescriptor

An object for requesting information from a user’s national ID card.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
class PKIdentityNationalIDCardDescriptor
```

## Mentioned in 

Requesting identity data from a Wallet pass

## Discussion

For the elements you request, the response contains the corresponding elements present in the user’s identity document. The table below maps the elements you request using PKIdentityElement with the ISO and JP namespace in the response.

Note

You can retrieve elements specific to Japan only when you have set the API region to `JP`.

| Identity element | ISO namespace | JP namespace |
|----|----|----|
| `givenName` |  | `full_name_unicode` |
| `familyName` |  | `full_name_unicode` |
| `portrait` |  | `portrait` |
| `address` |  | `resident_address_unicode, local_gov_code_unicode` |
| `documentNumber` |  | `individual_number_unicode` |
| `sex` | `sex` | `sex_unicode` |
| `age` | `age_in_years` |  |
| `dateOfBirth` | `birth_date` | `birth_date_unicode` |
| `age(atLeast: XX)` | `age_over_XX` |  |

This API requires a special entitlement issued by Apple. After you receive the entitlement, configure your Xcode project to use it:

1.  Add the entitlement to the property list specified in your target.

2.  In the `entitlements.plist` for the entitlement, add a new document-types item.

3.  Add a new element string.

Building an app with this entitlement requires macOS 13 or later. For more information about the entitlement, see Getting started with the Verify with Wallet API.

## Topics

### Setting region information

var region: Locale.Region?

A string used to specify the region associated with the ID.

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

### Japan passes

struct JPKIPassContents

A set of actions for viewing and updating PINs, passwords, and signing abilities associated with digital identities on the JPKI applet.

class PKAddIdentityDocumentConfiguration

Configuration to define the identity document.

class PKAddPassMetadataPreview

A preview object that contains information representing the pass you add to Wallet.

class PKIdentityDocumentMetadata

A set of configured metadata defining the required information to add the corresponding pass to Wallet.

class PKJapanIndividualNumberCardMetadata

A class that contains metadata indicating the specific product instance to provision.

