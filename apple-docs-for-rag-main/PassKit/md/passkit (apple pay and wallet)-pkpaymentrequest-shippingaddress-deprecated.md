

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  shippingAddress Deprecated

Instance Property

# shippingAddress

A prepopulated shipping address.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0Deprecated

``` source
unowned(unsafe) var shippingAddress: ABRecord? { get set }
```

Deprecated

This property is deprecated. Use the shippingContact property instead.

## Discussion

If you already have a shipping address on file, set this property to that address. When the PKPaymentAuthorizationViewController class is presented, the user can either keep the address you specified or enter a different address.

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

var billingAddress: ABRecord?

A prepopulated billing address.

Deprecated

