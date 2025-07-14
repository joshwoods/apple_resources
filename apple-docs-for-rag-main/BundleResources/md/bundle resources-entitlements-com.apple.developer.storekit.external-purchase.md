

- Bundle Resources
- Entitlements
-  com.apple.developer.storekit.external-purchase 

Property List Key

# com.apple.developer.storekit.external-purchase

A Boolean value that indicates whether your app can offer external purchases.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

## Details 

Type  

boolean

## Discussion

Qualifying apps may offer external purchases within the app. To offer external purchases in your app, complete a request for this entitlement. For more information about qualifying apps and to request this entitlement, see:

- Using alternative payment options on the App Store in the European Union

- Distributing dating apps in the Netherlands

- Distributing apps using a third-party payment provider in South Korea

If your account receives this entitlement, which is also known as the StoreKit External Purchase entitlement, add it to your app by opening the project’s .`entitlements` file in Xcode. Then add the following key and set the corresponding value to `true`:

```

    com.apple.developer.storekit.external-purchase

```

For more information, see External Purchase.

## See Also

### StoreKit

com.apple.developer.storekit.external-link.account

A Boolean value that indicates whether your app can link to an external website for account creation or management.

com.apple.developer.storekit.external-purchase-link

A Boolean value that indicates whether your app can include a link that directs people to a website to make an external purchase.

