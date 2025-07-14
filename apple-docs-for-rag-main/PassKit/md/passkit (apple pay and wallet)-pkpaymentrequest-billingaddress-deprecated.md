

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  billingAddress Deprecated

Instance Property

# billingAddress

A prepopulated billing address.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0Deprecated

``` source
unowned(unsafe) var billingAddress: ABRecord? { get set }
```

Deprecated

This property is deprecated. Use the billingContact property instead.

## Discussion

If you already have a billing address on file, set it here. The user can either use the address you specify or select a different address.

## See Also

### Deprecated

static var enabled: PKShippingContactEditingMode

All fields of the shipping contact on the payment sheet are editable by the user.

Deprecated

var requiredBillingAddressFields: PKAddressField

A bit field of billing address fields that you need in order to process the transaction.

Deprecated

var requiredShippingAddressFields: PKAddressField

A bit field of shipping address fields that you need in order to process the transaction.

Deprecated

struct PKAddressField

Billing or shipping address fields.

Deprecated

var shippingAddress: ABRecord?

A prepopulated shipping address.

Deprecated

