

- StoreKit
- ProductViewStyleConfiguration
-  descriptionVisibility 

Instance Property

# descriptionVisibility

The visibility of product descriptions.

StoreKitSwiftUIiOS 17.4+iPadOS 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
let descriptionVisibility: Visibility
```

## Discussion

Subscription products have a localized description property that you can conditionally display in your custom style. Use the descriptionVisibility property to check the value that the productDescription(_:) view modifier configures on an ancestor of the SubscriptionStoreView.

Ignore this property if your style doesn’t need the capability to conditionally display the product description. For example, a compact control style may never show product descriptions.

If the view heirarachy doesn’t use the productDescription(_:) view modifier, the descriptionVisibility property is automatic.

