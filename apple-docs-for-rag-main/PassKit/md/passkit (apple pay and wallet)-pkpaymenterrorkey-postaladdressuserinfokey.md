

- PassKit (Apple Pay and Wallet)
- PKPaymentErrorKey
-  postalAddressUserInfoKey 

Type Property

# postalAddressUserInfoKey

Payment error key that indicates errors with the postal address.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
static let postalAddressUserInfoKey: PKPaymentErrorKey
```

## Discussion

See CNPostalAddress for the values that can be used with this key. These values point to the specific area of the address that is at fault, for example, CNPostalAddressStreetKey indicates the street. When you supply the key values in a payment error, the Apple Pay sheet highlights the appropriate field, enabling the user to correct errors.

## See Also

### Error keys

static let contactFieldUserInfoKey: PKPaymentErrorKey

Payment error key that indicates errors with the contact information.

