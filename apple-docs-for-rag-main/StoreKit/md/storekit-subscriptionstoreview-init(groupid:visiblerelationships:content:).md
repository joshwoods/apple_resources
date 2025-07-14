

- StoreKit
- SubscriptionStoreView
-  init(groupID:visibleRelationships:content:) 

Initializer

# init(groupID:visibleRelationships:content:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    groupID: String,
    visibleRelationships: Product.SubscriptionRelationship = .all,
    @StoreContentBuilder content: () -> C
) where Content == SubscriptionStoreContentView, C : StoreContent
```

Available when `Content` conforms to `View`.

## See Also

### Creating subscription store views with a hierarchichal structure

init&lt;C>(productIDs: some Collection&lt;String>, content: () -> C)

init&lt;C>(subscriptions: some Collection&lt;Product>, content: () -> C)

