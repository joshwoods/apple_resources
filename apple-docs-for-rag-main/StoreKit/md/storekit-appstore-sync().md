

- StoreKit
- AppStore
-  sync() 

Type Method

# sync()

Synchronizes your app’s transaction information and subscription status with information from the App Store.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func sync() async throws
```

## Discussion

Include some mechanism in your app, such as a Restore Purchases button, to let users restore their in-app purchases. In rare cases when a user suspects the app isn’t showing all the transactions, call sync(). By calling sync(), you force the app to obtain transaction information and subscription status from the App Store.

Important

Calling sync()displays a system prompt that asks users to authenticate with their App Store credentials. Call this function only in response to an explicit user action, like tapping or clicking a button.

In regular operations, there’s no need to call sync(). StoreKit automatically keeps up to date transaction information and subscription status available to your app. When users reinstall your app or download it on a new device, the app automatically has all transactions available to it upon initial launch. There’s no need for users to ask your app to restore transactions — your app can immediately get the current entitlements using currentEntitlements and transaction history using all. For more information about transactions, see Transaction.

