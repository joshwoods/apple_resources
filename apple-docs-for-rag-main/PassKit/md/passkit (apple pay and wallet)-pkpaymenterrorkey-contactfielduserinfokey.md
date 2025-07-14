

- PassKit (Apple Pay and Wallet)
- PKPaymentErrorKey
-  contactFieldUserInfoKey 

Type Property

# contactFieldUserInfoKey

Payment error key that indicates errors with the contact information.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
static let contactFieldUserInfoKey: PKPaymentErrorKey
```

## Discussion

See PKContactField for the values to use with this key.

Use this key with the error code PKPaymentError.Code.shippingContactInvalidError to indicate an error in the name, email address, phone number, or the shipping address as a whole.

Use this key with the error code billingContactInvalidError to indicate an error with the billing address as a whole, or billing name.

The example code in Listing 1 shows the contactFieldUserInfoKey used to indicate a phone number error.

The following example shows an error indicating a problem with the shipping contact’s phone number.

```
let phoneError = NSError.init(domain: PKPaymentErrorDomain,
                               code: PKPaymentError.shippingContactInvalidError.rawValue,
                               userInfo: [NSLocalizedDescriptionKey:"Phone number is invalid",
                               PKPaymentErrorKey.contactFieldUserInfoKey:PKContactField.phoneNumber])
```

## See Also

### Error keys

static let postalAddressUserInfoKey: PKPaymentErrorKey

Payment error key that indicates errors with the postal address.

