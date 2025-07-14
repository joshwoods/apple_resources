

- StoreKit
- Product
- Product.SubscriptionInfo
-  status 

Instance Property

# status

An array that contains status information for a subscription group, including renewal and transaction information.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var status: [Product.SubscriptionInfo.Status] { get async throws }
```

## Discussion

This array is empty if the customer was never subscribed to a product in this subscription group.

The array can have more than one subscription status if your subscription supports Family Sharing. Provide the customer with service for the subscription based on the highest level of service where the state is subscribed.

## See Also

### Determining the subscription status

static func status(for: String) async throws -> [Product.SubscriptionInfo.Status]

Gets the subscription status for a subscription group identifier.

struct Status

The renewal status information for an auto-renewable subscription.

