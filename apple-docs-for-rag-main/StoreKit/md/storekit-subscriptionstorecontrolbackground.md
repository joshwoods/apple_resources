

- StoreKit
-  SubscriptionStoreControlBackground 

Structure

# SubscriptionStoreControlBackground

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+

``` source
struct SubscriptionStoreControlBackground
```

## Topics

### Background types

static var automatic: SubscriptionStoreControlBackground

static var gradientMaterial: SubscriptionStoreControlBackground

static var gradientMaterialOnScroll: SubscriptionStoreControlBackground

## See Also

### Adding backgrounds to subscription stores

nonisolated func containerBackground&lt;S>(_ style: S, for container: ContainerBackgroundPlacement) -> some View where S : ShapeStyle 

Sets the container background of the enclosing container using a view.

nonisolated func containerBackground&lt;V>(for container: ContainerBackgroundPlacement, alignment: Alignment = .center, @ViewBuilder content: () -> V) -> some View where V : View 

Sets the container background of the enclosing container using a view.

nonisolated func subscriptionStoreControlBackground(_ backgroundStyle: some ShapeStyle) -> some View 

Set a shape style to use for the background of subscription store view controls within the view.

nonisolated func subscriptionStoreControlBackground(_ backgroundStyle: SubscriptionStoreControlBackground) -> some View 

Set a standard effect to use for the background of subscription store view controls within the view.

static var subscriptionStore: ContainerBackgroundPlacement { get }

An automatic placement within a subscription store view, based on the view’s context.

static var subscriptionStoreHeader: ContainerBackgroundPlacement { get }

A background placement behind the marketing content of a subscription store view.

static var subscriptionStoreFullHeight: ContainerBackgroundPlacement { get }

A background placement that spans the full height of a subscription store view.

