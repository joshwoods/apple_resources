

- PassKit (Apple Pay and Wallet)
- PKPayment
-  billingAddress Deprecated

Instance Property

# billingAddress

The user-selected billing address for this transaction.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0Deprecated

``` source
unowned(unsafe) var billingAddress: ABRecord? { get }
```

Deprecated

This property is deprecated. Use billingContact instead.

## Discussion

Only the fields specified in the the requiredBillingAddressFields property of the PKPaymentRequest object are populated. If no required billing fields were specified, the value of this property is `nil`.

## See Also

### Deprecated

var shippingAddress: ABRecord?

The user-selected shipping address for this transaction.

Deprecated

