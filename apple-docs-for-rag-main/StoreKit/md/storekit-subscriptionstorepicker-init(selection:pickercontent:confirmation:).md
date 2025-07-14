

- StoreKit
- SubscriptionStorePicker
-  init(selection:pickerContent:confirmation:) 

Initializer

# init(selection:pickerContent:confirmation:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    selection: Binding,
    @ViewBuilder pickerContent: () -> PickerContent,
    @ViewBuilder confirmation: @escaping (SubscriptionStoreControlStyleConfiguration.Option) -> ConfirmationContent
)
```

Available when `PickerContent` conforms to `View` and `ConfirmationContent` conforms to `View`.

## See Also

### Managing a subscription picker’s selection state

init(SubscriptionStoreControlStyleConfiguration, selection: Binding&lt;SubscriptionStoreControlStyleConfiguration.Option?>, pickerOptionContent: (SubscriptionStoreControlStyleConfiguration.PickerOption) -> PickerContent, confirmation: (SubscriptionStoreControlStyleConfiguration.Option) -> ConfirmationContent)

