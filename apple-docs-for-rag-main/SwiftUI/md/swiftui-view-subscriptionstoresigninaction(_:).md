

- SwiftUI
- View
-  subscriptionStoreSignInAction(\_:) 

Instance Method

# subscriptionStoreSignInAction(\_:)

Adds an action to perform when a person uses the sign-in button on a subscription store view within a view.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func subscriptionStoreSignInAction(_ action: (() -> ())?) -> some View
```

## Parameters 

`action`  

The action to perform. Pass `nil` to remove the sign in action for subscription stores within this view. The default value is `nil`.

## Discussion

You can only have one sign in action for a view. If an ancestor view specifies a sign in action, using this modifier will replace the ancestor’s sign in action.

If the value is `nil`, subscription stores will never show a sign in button. You can also hide the sign in button without removing the action by using the storeButton(_:for:) modifier, providing signIn as the button kind.

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

