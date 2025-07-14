

- StoreKit
- SubscriptionStoreView
-  init(subscriptions:) 

Initializer

# init(subscriptions:)

Creates a view that displays a collection of subscription options, and merchandises them with automatic marketing content.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(subscriptions: some Collection) where Content == AutomaticSubscriptionStoreMarketingContent
```

## Parameters 

`subscriptions`  

A collection of auto-renewable subscription Product instances to merchandise. The auto-renewable subscriptions need to belong to the same subscription group.

## See Also

### Creating subscription store views with automatic marketing content

init(groupID: String, visibleRelationships: Product.SubscriptionRelationship)

Creates a view that loads all subscriptions in a subscription group from the App Store, and merchandises them with automatic marketing content.

init(productIDs: some Collection&lt;String>)

Creates a view that loads subscriptions based on a collection of product identifiers, and merchandises them with automatic marketing content.

