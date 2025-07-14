

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationStatus
-  PKPaymentAuthorizationStatus.invalidShippingPostalAddress Deprecated

Case

# PKPaymentAuthorizationStatus.invalidShippingPostalAddress

Invalid or unusable shipping address.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
case invalidShippingPostalAddress
```

Deprecated

Use PKPaymentAuthorizationResult with the PKPaymentAuthorizationStatus.failure status instead. Include the result of paymentShippingAddressInvalidError(withKey:localizedDescription:) in the errors array.

## See Also

### Payment authorization status constants

case success

Merchant successfully authorized the transaction, or the transaction is expected to succeed.

case failure

Merchant failed to authorize the transaction.

case invalidBillingPostalAddress

Invalid or unusable billing address.

Deprecated

case invalidShippingContact

Invalid or incomplete shipping contact.

Deprecated

case pinRequired

Transaction requires PIN entry.

case pinIncorrect

Incorrect PIN entered.

case pinLockout

PIN retry limit exceeded.

