

- PassKit (Apple Pay and Wallet)
- PKMerchantCapability
-  instantFundsOut 

Type Property

# instantFundsOut

The value that indicates the merchant supports disbursing funds using Instant Funds Out.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
static var instantFundsOut: PKMerchantCapability { get }
```

## Discussion

This capability indicates the merchant supports disbursing funds using Instant Funds Out (IFO), which means the recipient receives funds in minutes rather than days. Passing `PKMerchantCapabilityInstantFundsOut` into the init(merchantIdentifier:currency:region:supportedNetworks:merchantCapabilities:summaryItems:) indicates that the merchant is going to use IFO to facilitate the disbursement once the individual authenticates it.

## See Also

### Constants

static var threeDSecure: PKMerchantCapability

Support for the 3-D Secure protocol.

static var emv: PKMerchantCapability

Support for the EMV protocol.

static var credit: PKMerchantCapability

Support for credit cards.

static var debit: PKMerchantCapability

Support for debit cards.

