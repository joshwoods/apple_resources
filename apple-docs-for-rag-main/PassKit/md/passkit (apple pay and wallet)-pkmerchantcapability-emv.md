

- PassKit (Apple Pay and Wallet)
- PKMerchantCapability
-  emv 

Type Property

# emv

Support for the EMV protocol.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
static var emv: PKMerchantCapability { get }
```

## Discussion

Include this value only if you support China Union Pay transactions.

## See Also

### Constants

static var instantFundsOut: PKMerchantCapability

The value that indicates the merchant supports disbursing funds using Instant Funds Out.

static var threeDSecure: PKMerchantCapability

Support for the 3-D Secure protocol.

static var credit: PKMerchantCapability

Support for credit cards.

static var debit: PKMerchantCapability

Support for debit cards.

