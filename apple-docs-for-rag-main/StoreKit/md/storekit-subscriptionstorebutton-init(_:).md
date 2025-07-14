

- StoreKit
- SubscriptionStoreButton
-  init(\_:) 

Initializer

# init(\_:)

Creates a button with an automatic label that describes the subscription option and starts a subscribe interaction when someone selects the button.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(_ option: SubscriptionStoreControlStyleConfiguration.Option)
```

## Discussion

You receive SubscriptionStoreControlStyleConfiguration.Option values to initialize the subscribe button from the makeBody(configuration:) method of your custom subscription store control style.

