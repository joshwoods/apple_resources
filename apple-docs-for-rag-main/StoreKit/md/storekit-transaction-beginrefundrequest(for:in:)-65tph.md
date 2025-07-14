

- StoreKit
- Transaction
-  beginRefundRequest(for:in:) 

Type Method

# beginRefundRequest(for:in:)

Presents the refund request sheet for the specified transaction in a window scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor
static func beginRefundRequest(
    for transactionID: UInt64,
    in scene: UIWindowScene
) async throws -> Transaction.RefundRequestStatus
```

## Parameters 

`transactionID`  

The identifier of the transaction the user is requesting a refund for.

`scene`  

The UIWindowScene that the system displays the sheet on.

## Return Value

Transaction.RefundRequestStatus

## Mentioned in 

Testing refund requests

Choosing a StoreKit API for In-App Purchases

## Discussion

Call this function from account settings or a help menu to enable customers to request a refund for an in-app purchase within your app. When you call this function, the system displays a refund sheet with the customer’s purchase details and a list of reason codes for the customer to choose from. For design guidance, see Human Interface Guidelines > In-app purchase > Providing help with in-app purchases.

When a customer requests a refund for consumable in-app purchases through your app, the App Stores sends a `CONSUMPTION_REQUEST` notificationType to your server. If the customer provided consent, respond by sending consumption data to the App Store using the Send Consumption Information endpoint. If not, don’t respond to the `CONSUMPTION_REQUEST` notification.

The App Store takes up to 48 hours to either approve or deny a refund.

For information about setting up your server to receive notifications, see Enabling App Store Server Notifications.

Note

If your app uses SwiftUI, use refundRequestSheet(for:isPresented:onDismiss:) instead. For example usage, see Food Truck: Building a SwiftUI multiplatform app.

### Test refund requests

The sandbox environment and StoreKit Testing in Xcode both support testing refund requests. For more information, see Testing refund requests.

## See Also

### Requesting refunds

Testing refund requests

Test your app’s implementation of refund requests, and your app’s and server’s handling of approved and declined refunds.

func beginRefundRequest(in: UIWindowScene) async throws -> Transaction.RefundRequestStatus

Presents the refund request sheet for the transaction in a window scene.

func beginRefundRequest(in: NSViewController) async throws -> Transaction.RefundRequestStatus

Presents the refund request sheet for the transaction in a view controller.

static func beginRefundRequest(for: UInt64, in: NSViewController) async throws -> Transaction.RefundRequestStatus

Presents the refund request sheet for the specified transaction in a view controller.

enum RefundRequestError

The error codes for refund requests.

enum RefundRequestStatus

The status codes for refund requests.

