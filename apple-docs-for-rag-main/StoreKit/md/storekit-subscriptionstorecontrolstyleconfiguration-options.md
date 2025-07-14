

- StoreKit
- SubscriptionStoreControlStyleConfiguration
-  options 

Instance Property

# options

An array of subscription options for the subscription store view to merchandise.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var options: [SubscriptionStoreControlStyleConfiguration.Option] { get }
```

## Discussion

The options property is an array that contains the main content of your subscription store control style, including the auto-renewable subscription products. Use the properties of each options value to declare your control style. Provide a control that enables the customer to subscribe to each option in the array. Call the subscribe() method when the customer activates a control to subscribe.

Display only the subscription options that appear in the options array. Use the allOptions property to access information about all the options, for example, to compute comparisons between subscription options.

To hide and sort subscription options, use the initializer of the SubscriptionStoreView. The options array maintains the sort order, and includes only the options you provide to the subscription store view’s initializer. For example, the following code initializes the subscription store to contain only the subscription options that upgrade the customer’s current subscription:

```
SubscriptionStoreView(groupID: "SAMPLE", visibleRelationships: .upgrade)
```

If you configure a subscription store view to show the current auto-renewal preference, the options array contains the autoRenewPreference subscription product. There’s no need to specifically display the autoRenewPreference product in that case.

Note

A subscription store control style needs only one of the properties, options or sections. Use options if your style doesn’t support sections.

If you declare a subscription store view using SubscriptionOptionSection instances, this property flattens the section structure and ignores any header or footer views.

## See Also

### Getting subscription options to merchandise

var sections: [SubscriptionStoreControlStyleConfiguration.Section]

The subscription options to merchandise by sections.

struct Option

Properties of an auto-renewable subscription option to merchandise.

struct PickerOption

The properties of a picker option to use for selecting a subscription.

struct Section

The properties of a section of subscription options within a subscription store control.

struct Icon

A type-erased icon of a subscription option.

