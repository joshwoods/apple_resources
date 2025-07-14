

- StoreKit
- SubscriptionStoreView
-  init(productIDs:) 

Initializer

# init(productIDs:)

Creates a view that loads subscriptions based on a collection of product identifiers, and merchandises them with automatic marketing content.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(productIDs: some Collection) where Content == AutomaticSubscriptionStoreMarketingContent
```

## Parameters 

`productIDs`  

The product identifiers to load from the App Store.

## See Also

### Creating subscription store views with automatic marketing content

init(groupID: String, visibleRelationships: Product.SubscriptionRelationship)

Creates a view that loads all subscriptions in a subscription group from the App Store, and merchandises them with automatic marketing content.

init(subscriptions: some Collection&lt;Product>)

Creates a view that displays a collection of subscription options, and merchandises them with automatic marketing content.

