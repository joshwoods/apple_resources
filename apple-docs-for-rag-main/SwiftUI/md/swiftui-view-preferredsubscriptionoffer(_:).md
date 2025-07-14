

- SwiftUI
- View
-  preferredSubscriptionOffer(\_:) 

Instance Method

# preferredSubscriptionOffer(\_:)

Selects a subscription offer to apply to a purchase that a customer makes from a subscription store view, a store view, or a product view.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func preferredSubscriptionOffer(_ offer: @escaping (Product, Product.SubscriptionInfo, [Product.SubscriptionOffer]) -> Product.SubscriptionOffer?) -> some View
```

## Parameters 

`offer`  

A closure that returns the subscription offer to apply to the customer’s purchase.

## Discussion

Subscription stores within this view use the subscription offer you specify to configure the appearance of the subscription plans. ProductView doesn’t display the terms of a subscription offer in the UI, but you can still use this modifier to declare which offer product views within a view hierarchy apply to a purchase.

Offer preferences that use this modifier override offer preferences from ancestor views.

Important

Subscription offers in the Product.SubscriptionInfo object may contain offers the customer isn’t eligible for. Instead, use the eligibleOffers argument of the offer closure to select the offers to apply to the customer’s purchase.

If StoreKit determines that the customer is eligible for more than one offer, the system calls the `offer` closure before it draws the product on the subscription store view, or before the customer initiates a purchase on a store view or product view. Return the subscription offer to apply to the product, if any, to have system-provided UI reflect the discounted pricing terms under the selected offer.

If your `offer` closure returns nil, the system selects the introductory offer, if it exists, and if the customer is eligible for it.

The following code example sets the preferred subscription offer to the first offer the customer is eligible for:

```
import SwiftUI
import StoreKit

@available(iOS 18.0, macOS 15.0, tvOS 18.0, watchOS 11.0, visionOS 2.0, *)
struct MyView: View {

    var body: some View {
        SubscriptionStoreView(groupID: groupIdentifier)
            .preferredSubscriptionOffer { product, subscription, eligibleOffers in
                // Determine the offer to use from the list of eligibleOffers.
                // This example just uses the first offer.
                return eligibleOffers.first
            }
    }
}
```

## See Also

### Interacting with the App Store and Apple Music

func appStoreOverlay(isPresented: Binding&lt;Bool>, configuration: () -> SKOverlay.Configuration) -> some View

Presents a StoreKit overlay when a given condition is true.

func manageSubscriptionsSheet(isPresented: Binding&lt;Bool>) -> some View

func refundRequestSheet(for: Transaction.ID, isPresented: Binding&lt;Bool>, onDismiss: ((Result&lt;Transaction.RefundRequestStatus, Transaction.RefundRequestError>) -> ())?) -> some View

Display the refund request sheet for the given transaction.

func offerCodeRedemption(isPresented: Binding&lt;Bool>, onCompletion: (Result&lt;Void, any Error>) -> Void) -> some View

Presents a sheet that enables users to redeem subscription offer codes that you configure in App Store Connect.

func musicSubscriptionOffer(isPresented: Binding&lt;Bool>, options: MusicSubscriptionOffer.Options, onLoadCompletion: ((any Error)?) -> Void) -> some View

Initiates the process of presenting a sheet with subscription offers for Apple Music when the `isPresented` binding is `true`.

func currentEntitlementTask(for: String, priority: TaskPriority, action: (EntitlementTaskState&lt;VerificationResult&lt;Transaction>?>) async -> ()) -> some View

Declares the view as dependent on the entitlement of an In-App Purchase product, and returns a modified view.

func inAppPurchaseOptions(((Product) async -> Set&lt;Product.PurchaseOption>)?) -> some View

Add a function to call before initiating a purchase from StoreKit view within this view, providing a set of options for the purchase.

func manageSubscriptionsSheet(isPresented: Binding&lt;Bool>, subscriptionGroupID: String) -> some View

func onInAppPurchaseCompletion(perform: ((Product, Result&lt;Product.PurchaseResult, any Error>) async -> ())?) -> some View

Add an action to perform when a purchase initiated from a StoreKit view within this view completes.

func onInAppPurchaseStart(perform: ((Product) async -> ())?) -> some View

Add an action to perform when a user triggers the purchase button on a StoreKit view within this view.

func productIconBorder() -> some View

Adds a standard border to an in-app purchase product’s icon .

func productViewStyle(some ProductViewStyle) -> some View

Sets the style for In-App Purchase product views within a view.

func productDescription(Visibility) -> some View

Configure the visibility of labels displaying an in-app purchase product description within the view.

func storeButton(Visibility, for: StoreButtonKind...) -> some View

Specifies the visibility of auxiliary buttons that store view and subscription store view instances may use.

func storeProductTask(for: Product.ID, priority: TaskPriority, action: (Product.TaskState) async -> ()) -> some View

Declares the view as dependent on an In-App Purchase product and returns a modified view.

