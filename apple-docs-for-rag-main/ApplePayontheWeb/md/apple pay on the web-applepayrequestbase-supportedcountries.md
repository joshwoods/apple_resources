

- Apple Pay on the Web
- ApplePayRequestBase
-  supportedCountries 

Instance Property

# supportedCountries

A list of two-letter country codes for limiting payment to credit cards from specific countries or regions.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  supportedCountries;
```

## Discussion

Use the list of supported countries or regions to limit payment cards to those issued in specific countries or regions. Indicate the supported countries or regions by using ISO-3166 country codes.

The supportedCountries list doesn’t affect the currency for the transaction, and it applies to all payment cards in Wallet.

## See Also

### Setting the transaction information

countryCode

The merchant’s two-letter ISO-3166 country code.

merchantCapabilities

An array of the payment capabilities that the merchant supports, such as credit or debit card payments.

supportedNetworks

The payment networks the merchant provides to their customers.

