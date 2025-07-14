

- StoreKit
- SubscriptionStoreControlStyleConfiguration
-  descriptionVisibility 

Instance Property

# descriptionVisibility

The visibility of product descriptions.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var descriptionVisibility: Visibility { get }
```

## Discussion

Use this property if you choose to support configuring the description visibility in your custom style. It reflects the value that the ancestor view sets with the productDescription(_:) view modifier.

