

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  currencyCode 

Instance Property

# currencyCode

The three-letter ISO 4217 currency code that determines the currency the payment request uses.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var currencyCode: String { get set }
```

## Discussion

Set this property to the three-letter code for the currency used by this payment request. Apple Pay interprets the amounts provided by the summary items attached to this request as amounts in this currency.

The framework translates the currency code from the alphabetic code to the corresponding numeric code. The numeric code is passed to the Secure Element and appears in the encrypted payment data. For more information on the Secure Element, see A Payment Token Is Created When a Payment Is Authorized in Apple Pay Programming Guide.

## See Also

### Setting currency and region information

var supportedCountries: Set&lt;String>?

A list of ISO 3166 country codes to limit payments to cards from specific countries or regions.

var countryCode: String

The merchant’s two-letter ISO 3166 country code.

