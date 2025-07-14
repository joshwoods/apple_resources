

- StoreKit
- AppStore
-  presentOfferCodeRedeemSheet(from:) 

Type Method

# presentOfferCodeRedeemSheet(from:)

Displays a sheet in the view that enables users to redeem a subscription offer code that you configure in App Store Connect.

macOS 15.0+

``` source
@MainActor
static func presentOfferCodeRedeemSheet(from controller: NSViewController) async throws
```

## Parameters 

`controller`  

An NSViewController that StoreKit uses to display the offer code redemption sheet.

## Mentioned in 

Supporting subscription offer codes in your app

## Discussion

This method displays a system sheet in the view, where customers can enter and redeem subscription offer codes. Use this method if you generate subscription offer codes in App Store Connect and your app uses AppKit.

Important

Set up subscription offer codes in App Store Connect before calling this API. Customers can only redeem these offers in your app through the redemption sheet; don’t use a custom UI.

For more information on offer codes, see Supporting subscription offer codes in your app.

When customers redeem an offer code, StoreKit emits the resulting transaction in updates. Set up a transaction listener as soon as your app launches to receive new transactions while the app is running.

## See Also

### Presenting the offer code redemption sheet

Supporting subscription offer codes in your app

Provide subscription service for customers who redeem offer codes through the App Store or within your app.

static func presentOfferCodeRedeemSheet(in: UIWindowScene) async throws

Displays a sheet in the window scene that enables users to redeem a subscription offer code that you configure in App Store Connect.

nonisolated func offerCodeRedemption(isPresented: Binding&lt;Bool>, onCompletion: @escaping @MainActor (Result&lt;Void, any Error>) -> Void = { _ in }) -> some View 

Presents a sheet that enables users to redeem subscription offer codes that you configure in App Store Connect.

