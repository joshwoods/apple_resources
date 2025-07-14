

- StoreKit
- SubscriptionStoreView
-  init(subscriptions:marketingContent:) 

Initializer

# init(subscriptions:marketingContent:)

Creates a view that displays a collection of subscription options, and merchandises them with custom marketing content.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    subscriptions: some Collection,
    @ViewBuilder marketingContent: () -> Content
)
```

## Parameters 

`subscriptions`  

A collection of auto-renewable subscription Product instances to merchandise. The auto-renewable subscriptions need to belong to the same subscription group.

`marketingContent`  

A view that contains marketing content to display above the store controls.

## See Also

### Creating subscription store views with custom marketing content

init(groupID: String, visibleRelationships: Product.SubscriptionRelationship, marketingContent: () -> Content)

Creates a view that loads all the subscriptions in a subscription group from the App Store, and merchandises them with custom marketing content.

init(productIDs: some Collection&lt;String>, marketingContent: () -> Content)

Creates a view that loads a collection of subscriptions from the App Store, and merchandises them with custom marketing content.

