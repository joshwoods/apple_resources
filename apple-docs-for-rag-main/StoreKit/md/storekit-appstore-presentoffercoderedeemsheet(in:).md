

- StoreKit
- AppStore
-  presentOfferCodeRedeemSheet(in:) 

Type Method

# presentOfferCodeRedeemSheet(in:)

Displays a sheet in the window scene that enables users to redeem a subscription offer code that you configure in App Store Connect.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
static func presentOfferCodeRedeemSheet(in scene: UIWindowScene) async throws
```

## Parameters 

`scene`  

The UIWindowScene that StoreKit uses to display the offer code redemption sheet.

## Mentioned in 

Supporting subscription offer codes in your app

Implementing offer codes in your app

Testing purchases made outside your app

## Discussion

The presentOfferCodeRedeemSheet(in:) method displays a system sheet in the window scene, where customers can enter and redeem subscription offer codes. If you generate subscription offer codes in App Store Connect, call this function to enable users to redeem the offer. To display the sheet using SwiftUI, see offerCodeRedemption(isPresented:onCompletion:).

Important

Set up subscription offer codes in App Store Connect before calling this API. Customers can only redeem these offers in your app through the redemption sheet; don’t use a custom UI.

For more information on offer codes, see Supporting subscription offer codes in your app.

When customers redeem an offer code, StoreKit emits the resulting transaction in updates. Set up a transaction listener as soon as your app launches to receive new transactions while the app is running. For more information, see updates.

In Mac apps built with Mac Catalyst, this method throws a StoreKitError.unknown error.

## See Also

### Presenting the offer code redemption sheet

Supporting subscription offer codes in your app

Provide subscription service for customers who redeem offer codes through the App Store or within your app.

nonisolated func offerCodeRedemption(isPresented: Binding&lt;Bool>, onCompletion: @escaping @MainActor (Result&lt;Void, any Error>) -> Void = { _ in }) -> some View 

Presents a sheet that enables users to redeem subscription offer codes that you configure in App Store Connect.

static func presentOfferCodeRedeemSheet(from: NSViewController) async throws

Displays a sheet in the view that enables users to redeem a subscription offer code that you configure in App Store Connect.

