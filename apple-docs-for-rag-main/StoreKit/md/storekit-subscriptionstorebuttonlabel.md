

- StoreKit
-  SubscriptionStoreButtonLabel 

Structure

# SubscriptionStoreButtonLabel

The label of the subscribe button that a subscription store view uses.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
struct SubscriptionStoreButtonLabel
```

## Topics

### Instance Properties

var action: SubscriptionStoreButtonLabel

var displayName: SubscriptionStoreButtonLabel

var multiline: SubscriptionStoreButtonLabel

var price: SubscriptionStoreButtonLabel

var singleLine: SubscriptionStoreButtonLabel

### Type Properties

static var action: SubscriptionStoreButtonLabel

static var automatic: SubscriptionStoreButtonLabel

static var displayName: SubscriptionStoreButtonLabel

static var multiline: SubscriptionStoreButtonLabel

static var price: SubscriptionStoreButtonLabel

static var singleLine: SubscriptionStoreButtonLabel

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Configuring subscription store controls

nonisolated func subscriptionStoreControlIcon(@ViewBuilder icon: @escaping (Product, Product.SubscriptionInfo) -> some View) -> some View 

Sets a view to use to decorate individual subscription options within a subscription store view.

nonisolated func subscriptionStorePickerItemBackground(_ backgroundStyle: some ShapeStyle) -> some View 

Sets the background style for picker items of the subscription store view instances within a view.

nonisolated func subscriptionStorePickerItemBackground(_ backgroundStyle: some ShapeStyle, in shape: some Shape) -> some View 

Sets the background shape and style for subscription store view picker items within a view.

nonisolated func subscriptionStoreButtonLabel(_ label: SubscriptionStoreButtonLabel) -> some View 

Configures subscription store view instances within a view to use the provided button label.

