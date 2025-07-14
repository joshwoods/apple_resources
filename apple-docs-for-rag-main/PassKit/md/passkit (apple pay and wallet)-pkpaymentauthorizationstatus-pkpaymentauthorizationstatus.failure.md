

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationStatus
-  PKPaymentAuthorizationStatus.failure 

Case

# PKPaymentAuthorizationStatus.failure

Merchant failed to authorize the transaction.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
case failure
```

## Discussion

Use this value for all failures other than PIN-related failures (which have their own status constants), such as for an invalid address, contact, or unknown error.

List the specific errors in the errors array.

## See Also

### Payment authorization status constants

case success

Merchant successfully authorized the transaction, or the transaction is expected to succeed.

case invalidBillingPostalAddress

Invalid or unusable billing address.

Deprecated

case invalidShippingPostalAddress

Invalid or unusable shipping address.

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

