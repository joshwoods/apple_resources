

- Bundle Resources
- Entitlements
-  com.apple.developer.storekit.external-purchase-link 

Property List Key

# com.apple.developer.storekit.external-purchase-link

A Boolean value that indicates whether your app can include a link that directs people to a website to make an external purchase.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

## Details 

Type  

boolean

## Discussion

The com.apple.developer.storekit.external-purchase-link entitlement enables qualifying apps to include a link that directs people using the app to a website to make an external purchase. For more information about qualifying apps and to request this entitlement, see:

- Using alternative payment options on the App Store in the European Union

- Distributing dating apps in the Netherlands

- Distributing apps in Russia that provide an external purchase link

- Distributing apps in the U.S. that provide an external purchase link

- Distributing music streaming apps in the EEA that provide an external purchase link

If your account receives this entitlement, which is also known as the StoreKit External Purchase Link entitlement, you can add it to your app by opening the project’s `.entitlements` file in Xcode. Then add the following key and set the corresponding value to `true`:

```

    com.apple.developer.storekit.external-purchase-link

```

For more information, see External Purchase.

## See Also

### StoreKit

com.apple.developer.storekit.external-link.account

A Boolean value that indicates whether your app can link to an external website for account creation or management.

com.apple.developer.storekit.external-purchase

A Boolean value that indicates whether your app can offer external purchases.

