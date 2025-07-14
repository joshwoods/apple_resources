

- StoreKit Test
- SKTestSession
-  refundTransaction(identifier:) 

Instance Method

# refundTransaction(identifier:)

Simulates a refund for an in-app purchase that completes outside of the app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func refundTransaction(identifier: Int) throws
```

## Parameters 

`identifier`  

The transaction identifier of an in-app purchase to get a refund.

## Discussion

In the testing environment, the system always approves refund requests, and processes them immediately. You can choose the reason for the refund by using beginRefundRequest(in:) in your app and selecting a reason. (Your app may also use beginRefundRequest(for:in:), beginRefundRequest(in:), or beginRefundRequest(in:). If your app uses SwiftUI, it may use refundRequestSheet(for:isPresented:onDismiss:).) Otherwise, the refund reason defaults to other.

After calling this function, handle the new transaction in updates or in your payment queue. Look for the revocationDate and revocationReason properties, which indicate the refund.

## See Also

### Testing externally performed transactions

func buyProduct(productIdentifier: String) throws

Simulates buying an in-app purchase or subscription outside the app.

Deprecated

