

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  countryCode 

Instance Property

# countryCode

The merchant’s two-letter ISO 3166 country code.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var countryCode: String { get set }
```

## Discussion

Set this property to the two-letter ISO 3166 code for the country or region of the merchant’s principle place of business. This is often the location for settling the payment. The system stores the country code in the Secure Element as is. For more information on the Secure Element, see A Payment Token Is Created When a Payment Is Authorized in Apple Pay Programming Guide. Consult with your payment service provider (PSP) to determine the appropriate country code.

Apple Pay may use the `countryCode` to generate payment data that complies with local regulations. For more information on regional compliance, see Complying with regional regulations.

## See Also

### Setting currency and region information

var currencyCode: String

The three-letter ISO 4217 currency code that determines the currency the payment request uses.

var supportedCountries: Set&lt;String>?

A list of ISO 3166 country codes to limit payments to cards from specific countries or regions.

