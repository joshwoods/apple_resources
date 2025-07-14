

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  currency 

Instance Property

# currency

The currency to use for this disbursement.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS

``` source
var currency: Locale.Currency { get set }
```

## Discussion

Apple Pay interprets the amounts that this request’s summary items provide as amounts in this currency.

## See Also

### Setting currency and region information

var region: Locale.Region

The geographic region that describes the location for this disbursement.

var supportedRegions: [Locale.Region]?

An array of regions that describe the locations to support.

