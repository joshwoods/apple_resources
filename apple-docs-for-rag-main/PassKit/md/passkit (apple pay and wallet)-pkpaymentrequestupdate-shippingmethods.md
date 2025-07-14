

- PassKit (Apple Pay and Wallet)
- PKPaymentRequestUpdate
-  shippingMethods 

Instance Property

# shippingMethods

The list of shipping methods available for a payment request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
var shippingMethods: [PKShippingMethod] { get set }
```

## Discussion

The default value is an empty array that indicates there’s no update to the shipping methods.

