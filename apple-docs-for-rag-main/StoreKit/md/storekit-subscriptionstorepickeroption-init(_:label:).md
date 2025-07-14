

- StoreKit
- SubscriptionStorePickerOption
-  init(\_:label:) 

Initializer

# init(\_:label:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    _ option: SubscriptionStoreControlStyleConfiguration.Option,
    @ViewBuilder label: @escaping (SubscriptionStoreControlStyleConfiguration.PickerOption) -> Label
)
```

Available when `Label` conforms to `View`.

## See Also

### Creating a subscription picker option

init(SubscriptionStoreControlStyleConfiguration.Option)

init(SubscriptionStoreControlStyleConfiguration.PickerOption)

