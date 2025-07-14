

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationStatus
-  PKPaymentAuthorizationStatus.pinLockout 

Case

# PKPaymentAuthorizationStatus.pinLockout

PIN retry limit exceeded.

iOS 9.2+iPadOS 9.2+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
case pinLockout
```

## Discussion

Pass this constant to the completion block when the bank informs you that the user has exceeded the allowed number of attempts to enter their PIN.

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

case pinRequired

Transaction requires PIN entry.

case pinIncorrect

Incorrect PIN entered.

