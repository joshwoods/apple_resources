

- StoreKit
- SubscriptionStoreView
-  init(groupID:visibleRelationships:marketingContent:) 

Initializer

# init(groupID:visibleRelationships:marketingContent:)

Creates a view that loads all the subscriptions in a subscription group from the App Store, and merchandises them with custom marketing content.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    groupID: String,
    visibleRelationships: Product.SubscriptionRelationship = .all,
    @ViewBuilder marketingContent: () -> Content
)
```

## Parameters 

`groupID`  

The subscription group identifier to load from the App Store.

`visibleRelationships`  

The kinds of subscription option relationships the view makes visible when someone is already subscribed to the subscription.

`marketingContent`  

The view that contains marketing content to display above the store controls.

## See Also

### Creating subscription store views with custom marketing content

init(productIDs: some Collection&lt;String>, marketingContent: () -> Content)

Creates a view that loads a collection of subscriptions from the App Store, and merchandises them with custom marketing content.

init(subscriptions: some Collection&lt;Product>, marketingContent: () -> Content)

Creates a view that displays a collection of subscription options, and merchandises them with custom marketing content.

