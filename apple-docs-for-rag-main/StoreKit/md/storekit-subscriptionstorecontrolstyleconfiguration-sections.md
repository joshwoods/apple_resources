

- StoreKit
- SubscriptionStoreControlStyleConfiguration
-  sections 

Instance Property

# sections

The subscription options to merchandise by sections.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var sections: [SubscriptionStoreControlStyleConfiguration.Section] { get }
```

## Discussion

The sections property represents the main content of your subscription store control style, including the auto-renewable subscription products.

Each SubscriptionStoreControlStyleConfiguration.Section element contains an array of SubscriptionStoreControlStyleConfiguration.Option values named options. Use this structure to modify the appearance of a control depending on the section it belongs to.

The elements of sections represent SubscriptionOptionSection instances. A minimal store has one implicit section, with the sections property containing a single element. The single element’s header and footer properties are both `nil`, and its options property is identical to the options property on SubscriptionStoreControlStyleConfiguration.

Note

Typically, a style needs only one of the properties: options or sections. Use the sections property if your style supports sections.

Use the initializer of the SubscriptionStoreView to determine the contents of the sections array.

Display only the subscription options that appear in the sections array. Use the allOptions property to access information about all the options, for example, to compute comparisons between subscription options. The view your style creates needs to provide a control that enables the customer to subscribe to each option in the array.

If you configure a subscription store view to show the current auto-renewal preference, the sections array contains the autoRenewPreference subscription product. There’s no need to specifically display the autoRenewPreference product in that case.

## See Also

### Getting subscription options to merchandise

var options: [SubscriptionStoreControlStyleConfiguration.Option]

An array of subscription options for the subscription store view to merchandise.

struct Option

Properties of an auto-renewable subscription option to merchandise.

struct PickerOption

The properties of a picker option to use for selecting a subscription.

struct Section

The properties of a section of subscription options within a subscription store control.

struct Icon

A type-erased icon of a subscription option.

