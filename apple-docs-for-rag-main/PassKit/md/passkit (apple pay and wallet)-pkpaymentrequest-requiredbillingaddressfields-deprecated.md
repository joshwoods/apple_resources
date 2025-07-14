

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  requiredBillingAddressFields Deprecated

Instance Property

# requiredBillingAddressFields

A bit field of billing address fields that you need in order to process the transaction.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
var requiredBillingAddressFields: PKAddressField { get set }
```

Deprecated

This property is deprecated. Use requiredBillingContactFields instead.

## Discussion

The default value is PKPaymentRequest. For possible values, see PKPaymentRequest.

## See Also

### Deprecated

static var enabled: PKShippingContactEditingMode

All fields of the shipping contact on the payment sheet are editable by the user.

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

