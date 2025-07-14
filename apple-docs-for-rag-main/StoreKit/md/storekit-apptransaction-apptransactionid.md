

- StoreKit
- AppTransaction
-  appTransactionID 

Instance Property

# appTransactionID

The unique identifier of the app download transaction.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@backDeployed(before: iOS 18.4, macOS 15.4, tvOS 18.4, watchOS 11.4, visionOS 2.4)
var appTransactionID: String { get }
```

## Mentioned in 

Generating JWS to sign App Store requests

## Discussion

The App Store generates a single, globally unique `appTransactionID` for each Apple Account that downloads your app and for each family group member for apps that support Family Sharing.

This value remains the same for the same Apple Account and app if the customer redownloads the app on any device, receives a refund, repurchases the app, or changes the storefront. For apps that support Family Sharing, the `appTransactionID` is unique for each family group member.

The `appTransactionID` is available even if a customer makes no in-app purchases.

The App Store server and StoreKit provide the `appTransactionID` in the following APIs:

- This symbol, `appTransactionID`, in the AppTransaction object

- appTransactionID, in the subscription renewal information Product.SubscriptionInfo.RenewalInfo

- appTransactionID, in the transaction information Transaction

- In transaction and subscription renewal information you receive from notifications, App Store Server Notifications V2

- In transaction and subscription renewal information you receive from the App Store Server API

