

- SwiftUI
- View
-  transactionTask(\_:action:) 

Instance Method

# transactionTask(\_:action:)

Provides a task to perform before this view appears

SecureElementCredentialSwiftUIiOS 18.1+iPadOS 18.1+

``` source
nonisolated
func transactionTask(
    _ configuration: CredentialTransaction.Configuration?,
    action: @escaping (CredentialTransaction) async -> Void
) -> some View
```

## Parameters 

`configuration`  

A configuration containing information about the transaction task. When the task is completed or an error is encountered while performing the task, the system invalidates this configuration, and the `CredentialTransaction` is invalidated.

`action`  

A closure that will be called when `isPerformingTransaction` is `true`. It provides a `CredentialTransaction` instance that can be used to perform transactions.

## Discussion

This task provides an instance of a `CredentialTransaction` to be used to perform transactions.

A typical client should use the APIs in the following sequence:

1.  `acquirePresentmentIntentAssertion()` prior to showing any proprietary payment UI

2.  `relinquish()` the assertion before invoking the transaction API

3.  `configuration.invalidate()` after presenting the credential

4.  Optionally, `acquirePresentmentIntentAssertion()` to finish up any proprietary payment UI

5.  `relinquish()` the assertion

For example:

```
 struct TransactionView: View {
     @State private var configuration: CredentialTransaction.Configuration?
     private var assertion: PresentmentIntentAssertion // acquirePresentmentIntentAssertion() before transitioning into this view (step 1)
     private var activeSession: CredentialSession
     private var selectedCredential: Credential

     var body: some View {
         VStack {
             Button("Perform Transaction") {
                 guard let configuration else {
                    configuration = activeSession.configuration()
                    return
                 }

                 configuration.invalidate() // step 3
                 // Optional
                 assertion = try await session.acquirePresentmentIntentAssertion() // step 4
                 // handle any proprietary UI
                 try await assertion.relinquish() // step 5
                 // Optional end
             }
             .transactionTask(configuration) { transaction in
                 do {
                     try await assertion.relinquish() // step 2
                     try await transaction.performTransaction(using: selectedCredential)
                 } catch {
                     // code to handle error
                 }
             }
         }
     }
 }
```

## See Also

### Accessing Apple Pay and Wallet

@MainActor @preconcurrency struct PayWithApplePayButton&lt;Fallback> where Fallback : View

@MainActor @preconcurrency struct AddPassToWalletButton&lt;Fallback> where Fallback : View

@MainActor @preconcurrency struct VerifyIdentityWithWalletButton&lt;Fallback> where Fallback : View

A view that displays a button for identity verification.

func addOrderToWalletButtonStyle(AddOrderToWalletButtonStyle) -> some View

Sets the button’s style.

func addPassToWalletButtonStyle(AddPassToWalletButtonStyle) -> some View

Sets the style to be used by the button. (see `PKAddPassButtonStyle`).

func onApplePayCouponCodeChange(perform: (String) async -> PKPaymentRequestCouponCodeUpdate) -> some View

Called when a user has entered or updated a coupon code. This is required if the user is being asked to provide a coupon code.

func onApplePayPaymentMethodChange(perform: (PKPaymentMethod) async -> PKPaymentRequestPaymentMethodUpdate) -> some View

Called when a payment method has changed and asks for an update payment request. If this modifier isn’t provided Wallet will assume the payment method is valid.

func onApplePayShippingContactChange(perform: (PKContact) async -> PKPaymentRequestShippingContactUpdate) -> some View

Called when a user selected a shipping address. This is required if the user is being asked to provide a shipping contact.

func onApplePayShippingMethodChange(perform: (PKShippingMethod) async -> PKPaymentRequestShippingMethodUpdate) -> some View

Called when a user selected a shipping method. This is required if the user is being asked to provide a shipping method.

func payLaterViewAction(PayLaterViewAction) -> some View

Sets the action on the PayLaterView. See `PKPayLaterAction`.

func payLaterViewDisplayStyle(PayLaterViewDisplayStyle) -> some View

Sets the display style on the PayLaterView. See `PKPayLaterDisplayStyle`.

func payWithApplePayButtonStyle(PayWithApplePayButtonStyle) -> some View

Sets the style to be used by the button. (see `PayWithApplePayButtonStyle`).

func verifyIdentityWithWalletButtonStyle(VerifyIdentityWithWalletButtonStyle) -> some View

Sets the style to be used by the button. (see `PKIdentityButtonStyle`).

@MainActor @preconcurrency struct AsyncShareablePassConfiguration&lt;Content> where Content : View

