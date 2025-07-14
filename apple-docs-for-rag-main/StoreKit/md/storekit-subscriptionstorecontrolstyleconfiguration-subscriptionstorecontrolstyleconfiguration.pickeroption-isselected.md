

- StoreKit
- SubscriptionStoreControlStyleConfiguration
- SubscriptionStoreControlStyleConfiguration.PickerOption
-  isSelected 

Instance Property

# isSelected

A Boolean value that indicates whether the picker option is in a selected state.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
let isSelected: Bool
```

## Discussion

Use the isSelected property to display a selection indicator, such as a checkmark, in its correct state. The following code example shows a checkmark when isSelected is true:

```
SubscriptionPickerOption(option) { pickerOption in 
HStack {
    Text(pickerOption.displayName)
    Spacer()
    Image(systemName: "checkmark")
        .opacity(pickerOption.isSelected ? 1 : 0)
    }
}
```

The SubscriptionStorePicker automatically updates the picker’s selection state as customers interact with your picker. However, the SubscriptionStorePicker doesn’t display selection indicators. Your app needs to display selection indicators in the picker option label.

Use the SubscriptionStoreControlStyleConfiguration.PickerOption value, which represents the properties of a subscription picker option’s label, to display the selection indicator.

## See Also

### Getting properties of the subscription picker option

var subscription: Product

The auto-renewable subscription that the picker option represents.

var activeOffer: Product.SubscriptionOffer?

var icon: SubscriptionStoreControlStyleConfiguration.Icon?

The subscription option’s icon.

var id: Product.ID

