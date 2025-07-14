

- StoreKit
- SubscriptionStoreControlStyleConfiguration
- SubscriptionStoreControlStyleConfiguration.Section
-  options 

Instance Property

# options

The subscription options to merchandise within a section.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var options: [SubscriptionStoreControlStyleConfiguration.Option]
```

## Discussion

This property represents the main content of a section. The view your style creates needs to provide a control to subscribe to each option in the array.

Use the properties of each SubscriptionStoreControlStyleConfiguration.Option value to declare your control style, and use the subscribe() method in response to a subscribe interaction.

Tip

Use SubscriptionOptionSection to configure the contents of a section when creating a SubscriptionStoreView.

