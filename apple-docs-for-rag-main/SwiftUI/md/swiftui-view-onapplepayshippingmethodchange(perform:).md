

- SwiftUI
- View
-  onApplePayShippingMethodChange(perform:) 

Instance Method

# onApplePayShippingMethodChange(perform:)

Called when a user selected a shipping method. This is required if the user is being asked to provide a shipping method.

PassKitSwiftUIiOS 15.5+iPadOS 15.5+macOS 12.5+watchOS 8.5+

``` source
nonisolated
func onApplePayShippingMethodChange(perform action: @escaping (PKShippingMethod) async -> PKPaymentRequestShippingMethodUpdate) -> some View
```

## Return Value

An update to the payment request shipping method.

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

func payLaterViewAction(PayLaterViewAction) -> some View

Sets the action on the PayLaterView. See `PKPayLaterAction`.

func payLaterViewDisplayStyle(PayLaterViewDisplayStyle) -> some View

Sets the display style on the PayLaterView. See `PKPayLaterDisplayStyle`.

func payWithApplePayButtonStyle(PayWithApplePayButtonStyle) -> some View

Sets the style to be used by the button. (see `PayWithApplePayButtonStyle`).

func verifyIdentityWithWalletButtonStyle(VerifyIdentityWithWalletButtonStyle) -> some View

Sets the style to be used by the button. (see `PKIdentityButtonStyle`).

@MainActor @preconcurrency struct AsyncShareablePassConfiguration&lt;Content> where Content : View

func transactionTask(CredentialTransaction.Configuration?, action: (CredentialTransaction) async -> Void) -> some View

Provides a task to perform before this view appears

