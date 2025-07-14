

- StoreKit
- SubscriptionStorePicker
-  init(pickerContent:confirmation:) 

Initializer

# init(pickerContent:confirmation:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    @ViewBuilder pickerContent: () -> PickerContent,
    @ViewBuilder confirmation: @escaping (SubscriptionStoreControlStyleConfiguration.Option) -> ConfirmationContent
)
```

Available when `PickerContent` conforms to `View` and `ConfirmationContent` conforms to `View`.

## See Also

### Creating a subscription store picker

init(SubscriptionStoreControlStyleConfiguration, pickerOptionContent: (SubscriptionStoreControlStyleConfiguration.PickerOption) -> PickerContent, confirmation: (SubscriptionStoreControlStyleConfiguration.Option) -> ConfirmationContent)

