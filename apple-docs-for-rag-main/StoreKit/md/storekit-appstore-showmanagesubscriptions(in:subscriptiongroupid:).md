

- StoreKit
- AppStore
-  showManageSubscriptions(in:subscriptionGroupID:) 

Type Method

# showManageSubscriptions(in:subscriptionGroupID:)

Presents the App Store sheet for managing subscriptions for a subscription group.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
static func showManageSubscriptions(
    in scene: UIWindowScene,
    subscriptionGroupID: String
) async throws
```

## Parameters 

`scene`  

The UIWindowScene that the system displays the sheet on.

`subscriptionGroupID`  

The subscription group identifier that the subscription belongs to.

## Mentioned in 

Choosing a StoreKit API for In-App Purchases

## See Also

### Managing subscriptions

static func showManageSubscriptions(in: UIWindowScene) async throws

Presents the App Store sheet for managing subscriptions.

