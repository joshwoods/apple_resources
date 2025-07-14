

- StoreKit
- AppStore
-  showManageSubscriptions(in:) 

Type Method

# showManageSubscriptions(in:)

Presents the App Store sheet for managing subscriptions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
static func showManageSubscriptions(in scene: UIWindowScene) async throws
```

## Parameters 

`scene`  

The UIWindowScene that the system displays the sheet on.

## Mentioned in 

Testing In-App Purchases in Xcode

Testing failing subscription renewals and In-App Purchases

Testing win-back offers in Xcode

Testing at all stages of development with Xcode and the sandbox

## Discussion

Use this function to display the manage subscriptions sheet within your app. Consider adding a manage subscriptions option to your app. For design guidance on supporting this functionality, see Human Interface Guidelines > In-App Purchase > Helping People Manage Their Subscriptions.

The showManageSubscriptions(in:) function presents a manage subscription sheet that’s the same as what customers can view in their account settings in the App Store app or by choosing Settings \> Apple ID \> Subscriptions on an iOS or iPadOS device. The sheet displays the customer’s currently active subscription for your app and the options to view, upgrade, downgrade, or cancel their subscription.

If you’re using SwiftUI, call the manageSubscriptionsSheet(isPresented:)view modifier.

Avoid showing the user interface for this feature in Mac apps built with Mac Catalyst and on iOS apps running on Mac computers with Apple silicon because this sheet isn’t supported in macOS.

- In Mac apps built with Mac Catalyst, enclose the code in a compilation conditional block that uses the `targetEnvironment():` platform condition. For more information on Mac Catalyst, see Creating a Mac version of your iPad app.

- For iOS apps running on Apple silicon, if isiOSAppOnMac is `true,` avoid showing the user interface for this feature.

### Test managing subscriptions

Test the managing subscriptions functionality in the sandbox environment and StoreKit testing in Xcode. For more information about testing, see Testing at all stages of development with Xcode and the sandbox and Setting up StoreKit Testing in Xcode.

## See Also

### Managing subscriptions

static func showManageSubscriptions(in: UIWindowScene, subscriptionGroupID: String) async throws

Presents the App Store sheet for managing subscriptions for a subscription group.

