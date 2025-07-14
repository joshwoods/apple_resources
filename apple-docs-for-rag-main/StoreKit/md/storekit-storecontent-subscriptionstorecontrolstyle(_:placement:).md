

- StoreKit
- StoreContent
-  subscriptionStoreControlStyle(\_:placement:) 

Instance Method

# subscriptionStoreControlStyle(\_:placement:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func subscriptionStoreControlStyle(
    _ style: S,
    placement: S.Placement = .automatic
) -> some StoreContent where S : SubscriptionStoreControlStyle
```

## See Also

### Configuring store content

func subscriptionStoreOptionGroupStyle(some SubscriptionOptionGroupStyle) -> some StoreContent

func subscriptionStoreButtonLabel(SubscriptionStoreButtonLabel) -> some StoreContent

func storeButton(Visibility, for: StoreButtonKind...) -> some StoreContent

func productDescription(Visibility) -> some StoreContent

