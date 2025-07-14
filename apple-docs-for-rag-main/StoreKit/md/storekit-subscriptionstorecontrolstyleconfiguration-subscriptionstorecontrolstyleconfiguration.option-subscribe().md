

- StoreKit
- SubscriptionStoreControlStyleConfiguration
- SubscriptionStoreControlStyleConfiguration.Option
-  subscribe() 

Instance Method

# subscribe()

Initiates a purchase when a customer activates a control to subscribe to the option.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func subscribe()
```

## Discussion

Call the subscribe() method within your custom style when the customer chooses to make a purchase.

Important

Don’t call purchase methods, such as `Product/purchase(confirmIn:options:)`, on the subscription property from your custom style.

