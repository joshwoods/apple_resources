

- PassKit (Apple Pay and Wallet)
- PKShippingContactEditingMode
-  enabled Deprecated

Type Property

# enabled

All fields of the shipping contact on the payment sheet are editable by the user.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
static var enabled: PKShippingContactEditingMode { get }
```

Deprecated

Use PKShippingContactEditingMode.available instead.

## See Also

### Deprecated

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

var shippingAddress: ABRecord?

A prepopulated shipping address.

Deprecated

