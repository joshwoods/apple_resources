

- PassKit (Apple Pay and Wallet)
- PKAddressField
-  email Deprecated

Type Property

# email

The buyer’s email address.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOSvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
static var email: PKAddressField { get }
```

Deprecated

Use PKContactField and -requiredShippingContactFields / -requiredBillingContactFields

## See Also

### Constants

static var postalAddress: PKAddressField

The buyer’s full street address, including name, street, city, state or province, postal code, and country or region.

Deprecated

static var phone: PKAddressField

The buyer’s telephone number.

Deprecated

static var name: PKAddressField

The buyer’s first and last name.

static var all: PKAddressField

All fields.

Deprecated

