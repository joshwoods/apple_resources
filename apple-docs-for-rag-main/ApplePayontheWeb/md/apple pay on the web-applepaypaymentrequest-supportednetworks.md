

- Apple Pay on the Web
- ApplePayPaymentRequest
-  supportedNetworks 

Instance Property

# supportedNetworks

The payment networks the merchant supports.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required sequence  supportedNetworks;
```

## Discussion

You must set this property to one or more of the payment network values in the following table:

| Payment network   | Apple Pay version where first available |
|-------------------|-----------------------------------------|
| `amex`            | 1                                       |
| `bancomat`        | 14                                      |
| `bancontact`      | 14                                      |
| `cartesBancaires` | 4                                       |
| `chinaUnionPay`   | 1                                       |
| `dankort`         | 13                                      |
| `discover`        | 1                                       |
| `eftpos`          | 4                                       |
| `electron`        | 4                                       |
| `elo`             | 5                                       |
| `girocard`        | 11                                      |
| `interac`         | 1                                       |
| `jcb`             | 2                                       |
| `mada`            | 5                                       |
| `maestro`         | 4                                       |
| `masterCard`      | 1                                       |
| `mir`             | 11                                      |
| `privateLabel`    | 1                                       |
| `visa`            | 1                                       |
| `vPay`            | 4                                       |

To use a network introduced with a specific Apple Pay version, set the ApplePaySession version parameter to the required version number, like this:

```
```

For the best compatibility with operating systems and browsers, use the lowest possible version number that supports your payment networks and other required features.

In macOS 12.3, iOS 15.4, watchOS 8.5, and Mac Catalyst 15.4 or later, specify payment methods in the order you prefer. For example, to specify the default network to use for cobadged cards, set the first element in the array to the default network, and alternate networks afterward in the order you prefer.

Note

Websites supporting debit networks should check for regional regulations. For more information, see Complying with regional regulations.

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

supportedCountries

A list of two-letter country codes for limiting payment to cards from specific countries or regions.

ApplePayMerchantCapability

The payment capabilities the merchant supports.

ApplePayShippingMethod

A dictionary that describes the shipping method for delivering physical goods.

ApplePayShippingType

A type that indicates how to ship purchased items.

