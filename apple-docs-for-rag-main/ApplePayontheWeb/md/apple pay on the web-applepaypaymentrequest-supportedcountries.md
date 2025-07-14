

- Apple Pay on the Web
- ApplePayPaymentRequest
-  supportedCountries 

Instance Property

# supportedCountries

A list of two-letter country codes for limiting payment to cards from specific countries or regions.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  supportedCountries;
```

## Mentioned in 

Apple Pay on the Web Version 3 Release Notes

## Discussion

Use the list of supported countries or regions to limit payment cards to those issued in specific countries or regions. Indicate the supported countries or regions by using ISO 3166 country codes.

The supportedCountries list doesn’t affect the currency for the transaction, and it applies to all payment cards in Wallet.

## See Also

### Working with transaction information

countryCode

The merchant’s two-letter ISO 3166 country code.

currencyCode

The three-letter ISO 4217 currency code for the payment.

merchantCapabilities

An array of the payment capabilities that the merchant supports, such as credit or debit.

shippingMethods

The list of shipping methods available for a payment request.

shippingType

An optional value that indicates how to ship purchased items.

supportedNetworks

The payment networks the merchant supports.

ApplePayMerchantCapability

The payment capabilities the merchant supports.

ApplePayShippingMethod

A dictionary that describes the shipping method for delivering physical goods.

ApplePayShippingType

A type that indicates how to ship purchased items.

