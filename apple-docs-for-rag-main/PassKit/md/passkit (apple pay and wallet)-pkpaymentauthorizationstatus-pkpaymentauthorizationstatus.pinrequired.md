

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationStatus
-  PKPaymentAuthorizationStatus.pinRequired 

Case

# PKPaymentAuthorizationStatus.pinRequired

Transaction requires PIN entry.

iOS 9.2+iPadOS 9.2+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
case pinRequired
```

## Discussion

Pass this constant to the completion block when the payment requires a PIN but the token did not include one—for example, when the bank’s and app’s PIN limits are out of sync. Apple Pay automatically prompts the user to enter their PIN.

## See Also

### Payment authorization status constants

case success

Merchant successfully authorized the transaction, or the transaction is expected to succeed.

case failure

Merchant failed to authorize the transaction.

case invalidBillingPostalAddress

Invalid or unusable billing address.

Deprecated

case invalidShippingPostalAddress

Invalid or unusable shipping address.

Deprecated

case invalidShippingContact

Invalid or incomplete shipping contact.

Deprecated

case pinIncorrect

Incorrect PIN entered.

case pinLockout

PIN retry limit exceeded.

