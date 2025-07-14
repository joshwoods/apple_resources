

- Apple Pay on the Web
- ApplePayPaymentRequest
-  currencyCode 

Instance Property

# currencyCode

The three-letter ISO 4217 currency code for the payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required DOMString currencyCode;
```

## Discussion

Set this property to the three-letter code for the currency used by this payment request. Apple Pay interprets the amounts provided in the summary items of this request as amounts in this currency.

The currency code is validated.

## See Also

### Working with transaction information

countryCode

The merchant’s two-letter ISO 3166 country code.

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

