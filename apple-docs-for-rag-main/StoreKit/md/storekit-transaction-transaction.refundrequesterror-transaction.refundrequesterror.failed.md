

- StoreKit
- Transaction
- Transaction.RefundRequestError
-  Transaction.RefundRequestError.failed 

Case

# Transaction.RefundRequestError.failed

The refund request submission failed.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case failed
```

## Discussion

A refund request submission can fail for many reasons, such as having an invalid transaction identifier, or if the App Store can’t process the request for some other reason.

## See Also

### Error Enumeration

case duplicateRequest

The App Store has already received a refund request for this in-app purchase.

