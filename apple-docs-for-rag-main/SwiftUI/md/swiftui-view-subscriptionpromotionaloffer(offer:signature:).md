

- SwiftUI
- View
-  subscriptionPromotionalOffer(offer:signature:) 

Instance Method

# subscriptionPromotionalOffer(offer:signature:)

Selects a promotional offer to apply to a purchase a customer makes from a subscription store view.

StoreKitSwiftUIiOS 17.4+iPadOS 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
nonisolated
func subscriptionPromotionalOffer(
    offer: @escaping (Product, Product.SubscriptionInfo) -> Product.SubscriptionOffer?,
    signature: @escaping (Product, Product.SubscriptionInfo, Product.SubscriptionOffer) async throws -> Product.SubscriptionOffer.Signature
) -> some View
```

## Parameters 

`offer`  

The system calls this function before drawing the given subscription product on the subscription store view. Return the promotional offer to apply to the product, if any, to have system-provided UI reflect the discounted terms under the selected offer.

`signature`  

The system calls this function before processing a purchase, with the product to be purchased provided as a parameter, along with the selected subscription offer to be applied to the purchase. Return a signature you generate on your server that validates the selected offer. Errors thrown from this closure will be surfaced via the onInAppPurchaseCompletion(perform:) modifier. For information about generating the signature, see Generating a signature for promotional offers.

## Discussion

Subscription stores within this view uses the specified subscription offer to configure the appearance of the subscription plans displayed, when you use a system-provided SubscriptionStoreControlStyle to style the in-app subscription store. Standard ProductViewStyle instances don’t show introductory or promotional offers in UI. Use the SubscriptionStoreView instead to show these offers in the UI.

If the signature passes validation for the offer you select, the system applies the offer to the purchase. If the signature fails validation for the offer you select, the purchase fails with Product.PurchaseError.invalidOfferSignature.

Promotional offers you select in this modifier overwrite any offers you specified in ancestor views.

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

