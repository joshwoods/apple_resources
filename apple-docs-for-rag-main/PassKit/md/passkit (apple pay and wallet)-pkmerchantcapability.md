

- PassKit (Apple Pay and Wallet)
-  PKMerchantCapability 

Structure

# PKMerchantCapability

Capabilities for processing payment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
struct PKMerchantCapability
```

## Topics

### Initializers

init(rawValue: UInt)

Creates a merchant capability using the raw value you provide.

### Constants

static var instantFundsOut: PKMerchantCapability

The value that indicates the merchant supports disbursing funds using Instant Funds Out.

static var threeDSecure: PKMerchantCapability

Support for the 3-D Secure protocol.

static var emv: PKMerchantCapability

Support for the EMV protocol.

static var credit: PKMerchantCapability

Support for credit cards.

static var debit: PKMerchantCapability

Support for debit cards.

### Type Properties

static var capability3DS: PKMerchantCapability

static var capabilityCredit: PKMerchantCapability

static var capabilityDebit: PKMerchantCapability

static var capabilityEMV: PKMerchantCapability

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

### Setting merchant information

struct MerchantCategoryCode

An optional four-digit struct, in ISO 18245 format, that represents the type of goods or service the merchant provides for the transaction.

var merchantIdentifier: String

Your merchant identifier.

var merchantCapabilities: PKMerchantCapability

A bit field of the payment-processing protocols and card types that you support.

