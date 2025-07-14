

- PassKit (Apple Pay and Wallet)
- PKAddressField
-  name 

Type Property

# name

The buyer’s first and last name.

iOS 8.3–11.0DeprecatediPadOS 8.3–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
static var name: PKAddressField { get }
```

## Discussion

This constant lets you request the name used for shipping or billing. The name is also included as part of the postal address field. The system only handles the name as a separate field when the postal address is not requested.

## See Also

### Constants

static var postalAddress: PKAddressField

The buyer’s full street address, including name, street, city, state or province, postal code, and country or region.

Deprecated

static var phone: PKAddressField

The buyer’s telephone number.

Deprecated

static var email: PKAddressField

The buyer’s email address.

Deprecated

static var all: PKAddressField

All fields.

Deprecated

