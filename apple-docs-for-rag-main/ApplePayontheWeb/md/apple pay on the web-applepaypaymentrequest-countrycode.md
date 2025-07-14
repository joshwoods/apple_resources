

- Apple Pay on the Web
- ApplePayPaymentRequest
-  countryCode 

Instance Property

# countryCode

The merchant’s two-letter ISO 3166 country code.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required DOMString countryCode;
```

## Discussion

Set this property to the two-letter ISO 3166 code for the country or region of the merchant’s principle place of business. This is often the location for settling the payment. Consult with your payment service provider (PSP) to determine the appropriate country code.

Apple Pay may use the `countryCode` to generate payment data that complies with local regulations. For more information on regional compliance, see Complying with regional regulations.

## See Also

### Working with transaction information

currencyCode

The three-letter ISO 4217 currency code for the payment.

merchantCapabilities

An array of the payment capabilities that the merchant supports, such as credit or debit.

shippingMethods

The list of shipping methods available for a payment request.

shippingType

An optional value that indicates how to ship purchased items.

supportedCountries

A list of two-letter country codes for limiting payment to cards from specific countries or regions.

supportedNetworks

The payment networks the merchant supports.

ApplePayMerchantCapability

The payment capabilities the merchant supports.

ApplePayShippingMethod

A dictionary that describes the shipping method for delivering physical goods.

ApplePayShippingType

A type that indicates how to ship purchased items.

