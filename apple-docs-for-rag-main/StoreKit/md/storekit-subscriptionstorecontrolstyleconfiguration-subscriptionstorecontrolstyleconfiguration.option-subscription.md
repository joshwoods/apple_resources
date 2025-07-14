

- StoreKit
- SubscriptionStoreControlStyleConfiguration
- SubscriptionStoreControlStyleConfiguration.Option
-  subscription 

Instance Property

# subscription

The auto-renewable subscription to merchandise.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var subscription: Product { get }
```

## Discussion

SubscriptionStoreControlStyleConfiguration.Option is a dynamic member lookup type, which code refers to as `Option` when it’s a nested type. You don’t need to use the subscription property directly to access the properties of the Product value. Instead, access any properties of Product or Product.SubscriptionInfo directly on the `Option` value.

The following code example creates a button for each subscription option and displays its name. The displayName property is available on SubscriptionStoreControlStyleConfiguration.Option to use as the button label.

```
struct DisplayNameButtonsControlStyle: SubscriptionStoreControlStyle {

    func makeBody(configuration: Configuration) -> some View {
        ForEach(configuration.options) { option in
            Button(option.displayName, action: option.subscribe)
        }
    }
}
```

Important

Use the subscribe() method on the SubscriptionStoreControlStyleConfiguration.Option value when a customer initiates a purchase. Don’t use `Product/purchase(confirmIn:options:)` or related purchase methods on this property for initiating a purchase.

## See Also

### Getting the subscription product and offer

var id: Product.ID

The product ID of the auto-renewable subscription.

var activeOffer: Product.SubscriptionOffer?

The subscription offer the customer is eligible for, and that applies to the subscription option.

