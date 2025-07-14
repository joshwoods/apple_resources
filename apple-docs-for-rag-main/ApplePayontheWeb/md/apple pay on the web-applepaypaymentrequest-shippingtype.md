

- Apple Pay on the Web
- ApplePayPaymentRequest
-  shippingType 

Instance Property

# shippingType

An optional value that indicates how to ship purchased items.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayShippingType shippingType;
```

## Discussion

The shipping type is optional. If it is specified, it must be one or more of these values:

- `shipping`

- `delivery`

- `storePickup`

- `servicePickup`

The default value is `shipping`.

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

