

- Apple Pay on the Web
- ApplePayPaymentRequest
-  merchantCapabilities 

Instance Property

# merchantCapabilities

An array of the payment capabilities that the merchant supports, such as credit or debit.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required sequence  merchantCapabilities;
```

## Discussion

The supported values for `merchantCapabilities` are:

- `supports3DS` - Required. This value must be supplied.

- `supportsCredit` - Optional. If present, only transactions that are categorized as credit cards are allowed.

- `supportsDebit` - Optional. If present, only transactions that are categorized as debit cards are allowed.

- `supportsEMV` - Include this value only if you support China Union Pay transactions.

If both or neither `supportsCredit` and `supportsDebit` values are supplied, the transaction allows both credit and debit cards.

## See Also

### Working with transaction information

countryCode

The merchant’s two-letter ISO 3166 country code.

currencyCode

The three-letter ISO 4217 currency code for the payment.

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

