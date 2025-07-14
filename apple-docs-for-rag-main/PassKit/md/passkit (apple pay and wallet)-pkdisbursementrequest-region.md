

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  region 

Instance Property

# region

The geographic region that describes the location for this disbursement.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS

``` source
var region: Locale.Region { get set }
```

## Discussion

Set this property to the Locale.Region for the country or region of the merchant’s principal place of business. Consult with your payment service provider (PSP) to determine the appropriate country or region code.

Apple Pay may use the `region` to generate payment and disbursement data that complies with local regulations. For more information on regional compliance, see Complying with regional regulations.

## See Also

### Setting currency and region information

var currency: Locale.Currency

The currency to use for this disbursement.

var supportedRegions: [Locale.Region]?

An array of regions that describe the locations to support.

