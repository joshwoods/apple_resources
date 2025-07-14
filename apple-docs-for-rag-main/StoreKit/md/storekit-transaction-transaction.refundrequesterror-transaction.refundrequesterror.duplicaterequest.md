

- StoreKit
- Transaction
- Transaction.RefundRequestError
-  Transaction.RefundRequestError.duplicateRequest 

Case

# Transaction.RefundRequestError.duplicateRequest

The App Store has already received a refund request for this in-app purchase.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case duplicateRequest
```

## Discussion

StoreKit returns this error if the App Store has previously received a refund request for this transaction and the refund decision is still pending, has been previously denied, or has been previously approved.

Consider checking the transaction’s revocationDate or revocationReason before calling beginRefundRequest(for:in:) to identify whether the App Store has already refunded the transaction.

## See Also

### Error Enumeration

case failed

The refund request submission failed.

