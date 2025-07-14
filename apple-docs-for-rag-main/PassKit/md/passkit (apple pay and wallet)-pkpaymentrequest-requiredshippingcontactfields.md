

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  requiredShippingContactFields 

Instance Property

# requiredShippingContactFields

A list of fields that you need for a shipping contact to process the transaction.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var requiredShippingContactFields: Set { get set }
```

## Mentioned in 

Displaying a Read-Only Pickup Address

## Discussion

See PKContactField for the list of possible contact fields.

## See Also

### Requesting billing and shipping contact fields

var requiredBillingContactFields: Set&lt;PKContactField>

A list of fields that you need for a billing contact to process the transaction.

struct PKContactField

The fields that describe a contact.

