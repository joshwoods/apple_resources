

- SwiftUI
- View
-  currentEntitlementTask(for:priority:action:) 

Instance Method

# currentEntitlementTask(for:priority:action:)

Declares the view as dependent on the entitlement of an In-App Purchase product, and returns a modified view.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func currentEntitlementTask(
    for productID: String,
    priority: TaskPriority = .medium,
    action: @escaping (EntitlementTaskState?>) async -> ()
) -> some View
```

## Parameters 

`productID`  

The product ID to get the entitlement for. The task restarts whenever this parameter changes.

`priority`  

The task priority to use when creating the task.

`action`  

The action to perform when the task’s state changes.

## Discussion

Before a view modified with this method appears, a task will start in the background to get the current entitlement. While the view is presented, the task will call `action` whenever the entitlement changes or the task’s state changes.

Consumable in-app purchases will always pass `nil` to `action`. For auto-renewable subscriptions, use `subscriptionStatusTask(for:priority:action:)` to get the full status information for the subscription.

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

func storeProductsTask(for: some Collection&lt;String> &amp; Equatable &amp; Sendable, priority: TaskPriority, action: (Product.CollectionTaskState) async -> ()) -> some View

Declares the view as dependent on a collection of In-App Purchase products and returns a modified view.

