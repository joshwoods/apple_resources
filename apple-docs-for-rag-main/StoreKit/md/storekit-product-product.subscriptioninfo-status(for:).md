

- StoreKit
- Product
- Product.SubscriptionInfo
-  status(for:) 

Type Method

# status(for:)

Gets the subscription status for a subscription group identifier.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func status(for groupID: String) async throws -> [Product.SubscriptionInfo.Status]
```

## Parameters 

`groupID`  

The subscription group identifier of the subscription to get status for.

## Return Value

An array of Product.SubscriptionInfo.Status. This array is empty if the customer has never subscribed to a product in this subscription group.

## Discussion

To get the subscription group identifier of a subscription, see subscriptionGroupID in Product.SubscriptionInfo, or subscriptionGroupID in Transaction. You originally create subscription group identifiers when you set up in-app purchases in App Store Connect. For more information, see Offer auto-renewable subscriptions.

Users can only buy one auto-renewable subscription within a group at a time. However, the returned array may contain multiple status values if your subscription supports Family Sharing, and the person has access to other subscriptions in the group through Family Sharing. For more information about Family Sharing, see Enable Family Sharing for your subscriptions.

## See Also

### Determining the subscription status

var status: [Product.SubscriptionInfo.Status]

An array that contains status information for a subscription group, including renewal and transaction information.

struct Status

The renewal status information for an auto-renewable subscription.

