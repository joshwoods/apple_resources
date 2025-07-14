

- PassKit (Apple Pay and Wallet)
-  PKAddressField Deprecated

Structure

# PKAddressField

Billing or shipping address fields.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOSvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
struct PKAddressField
```

Deprecated

This field is deprecated. Use PKContactField instead.

## Topics

### Constants

static var postalAddress: PKAddressField

The buyer’s full street address, including name, street, city, state or province, postal code, and country or region.

static var phone: PKAddressField

The buyer’s telephone number.

static var email: PKAddressField

The buyer’s email address.

static var name: PKAddressField

The buyer’s first and last name.

static var all: PKAddressField

All fields.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Deprecated

var applePayLaterAvailability: PKPaymentRequest.ApplePayLaterAvailability

A value that indicates whether Apple Pay Later is available for a transaction.

Deprecated

enum ApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

enum PKApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

