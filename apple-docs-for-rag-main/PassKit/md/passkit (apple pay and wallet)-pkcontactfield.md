

- PassKit (Apple Pay and Wallet)
-  PKContactField 

Structure

# PKContactField

The fields that describe a contact.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct PKContactField
```

## Discussion

Use PKContactField field types to indicate which contact fields you require for a billing or shipping contact in order to complete the transaction.

## Topics

### Initializing a contact field

init(rawValue: String)

Create a contact field given the raw value.

### Types of contact fields

static let emailAddress: PKContactField

A constant that indicates a contact’s email address.

static let name: PKContactField

A constant that indicates a contact’s name.

static let phoneNumber: PKContactField

A constant that indicates a contact’s telephone number.

static let phoneticName: PKContactField

A constant that indicates a contact’s phonetic name.

static let postalAddress: PKContactField

A constant that indicates a contact’s postal address.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Requesting billing and shipping contact fields

var requiredBillingContactFields: Set&lt;PKContactField>

A list of fields that you need for a billing contact to process the transaction.

var requiredShippingContactFields: Set&lt;PKContactField>

A list of fields that you need for a shipping contact to process the transaction.

