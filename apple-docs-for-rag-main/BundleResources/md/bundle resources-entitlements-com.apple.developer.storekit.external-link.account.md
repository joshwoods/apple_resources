

- Bundle Resources
- Entitlements
-  com.apple.developer.storekit.external-link.account 

Property List Key

# com.apple.developer.storekit.external-link.account

A Boolean value that indicates whether your app can link to an external website for account creation or management.

iOS 15.4+iPadOS 15.4+tvOS 16.4+

## Details 

Type  

boolean

## Discussion

If your developer account has this entitlement, add it to your app by opening the project’s entitlements file in Xcode. Add the following key and set the corresponding value to `true`:

```

    com.apple.developer.storekit.external-link.account

```

## See Also

### StoreKit

com.apple.developer.storekit.external-purchase

A Boolean value that indicates whether your app can offer external purchases.

com.apple.developer.storekit.external-purchase-link

A Boolean value that indicates whether your app can include a link that directs people to a website to make an external purchase.

