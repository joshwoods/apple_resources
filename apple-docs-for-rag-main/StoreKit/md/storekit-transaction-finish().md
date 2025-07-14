

- StoreKit
- Transaction
-  finish() 

Instance Method

# finish()

Indicates to the App Store that the app delivered the purchased content or enabled the service to finish the transaction.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func finish() async
```

## Mentioned in 

Supporting win-back offers in your app

Supporting subscription offer codes in your app

Testing at all stages of development with Xcode and the sandbox

Supporting promoted In-App Purchases in your app

## Discussion

Call finish() to complete a transaction after you deliver the purchased content or enable the purchased service. For on-demand resources, don’t finish the transaction until the app completes downloading the resource or you’ve otherwise delivered the resource.

## See Also

### Finishing the transaction

static var unfinished: Transaction.Transactions

A sequence that emits unfinished transactions for the customer.

