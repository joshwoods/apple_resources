

- StoreKit
- SubscriptionStoreView
-  init(productIDs:content:) 

Initializer

# init(productIDs:content:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    productIDs: some Collection,
    @StoreContentBuilder content: () -> C
) where Content == SubscriptionStoreContentView, C : StoreContent
```

Available when `Content` conforms to `View`.

## See Also

### Creating subscription store views with a hierarchichal structure

init&lt;C>(groupID: String, visibleRelationships: Product.SubscriptionRelationship, content: () -> C)

init&lt;C>(subscriptions: some Collection&lt;Product>, content: () -> C)

