

- StoreKit
- SubscriptionStorePicker
-  init(\_:selection:pickerOptionContent:confirmation:) 

Initializer

# init(\_:selection:pickerOptionContent:confirmation:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    _ configuration: SubscriptionStoreControlStyleConfiguration,
    selection: Binding,
    @ViewBuilder pickerOptionContent: @escaping (SubscriptionStoreControlStyleConfiguration.PickerOption) -> PickerContent,
    @ViewBuilder confirmation: @escaping (SubscriptionStoreControlStyleConfiguration.Option) -> ConfirmationContent
)
```

Available when `PickerContent` conforms to `View` and `ConfirmationContent` conforms to `View`.

## See Also

### Managing a subscription picker’s selection state

init(selection: Binding&lt;SubscriptionStoreControlStyleConfiguration.Option?>, pickerContent: () -> PickerContent, confirmation: (SubscriptionStoreControlStyleConfiguration.Option) -> ConfirmationContent)

