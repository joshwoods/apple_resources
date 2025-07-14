

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationStatus
-  PKPaymentAuthorizationStatus.pinIncorrect 

Case

# PKPaymentAuthorizationStatus.pinIncorrect

Incorrect PIN entered.

iOS 9.2+iPadOS 9.2+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
case pinIncorrect
```

## Discussion

Pass this constant to the completion block when the payment token includes an invalid PIN number. Apple Pay automatically prompts the user to reenter their PIN.

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

case pinLockout

PIN retry limit exceeded.

