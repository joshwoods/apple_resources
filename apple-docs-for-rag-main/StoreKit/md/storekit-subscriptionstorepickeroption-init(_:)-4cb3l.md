

- StoreKit
- SubscriptionStorePickerOption
-  init(\_:) 

Initializer

# init(\_:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(_ option: SubscriptionStoreControlStyleConfiguration.Option) where Label == AutomaticSubscriptionStorePickerOptionLabel
```

Available when `Label` conforms to `View`.

## See Also

### Creating a subscription picker option

init(SubscriptionStoreControlStyleConfiguration.PickerOption)

init(SubscriptionStoreControlStyleConfiguration.Option, label: (SubscriptionStoreControlStyleConfiguration.PickerOption) -> Label)

