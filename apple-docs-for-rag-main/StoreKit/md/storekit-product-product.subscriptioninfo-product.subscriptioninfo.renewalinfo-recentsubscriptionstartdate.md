

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  recentSubscriptionStartDate 

Instance Property

# recentSubscriptionStartDate

The earliest start date of a subscription in a series of auto-renewable subscription purchases that ignores all lapses of paid service shorter than 60 days.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@backDeployed(before: iOS 16.0, macOS 13.0, tvOS 16.0, watchOS 9.0, macCatalyst 16.0)
var recentSubscriptionStartDate: Date { get }
```

## Discussion

Important

Don’t use the recentSubscriptionStartDate date to calculate days of paid service. For more information about paid days of service, see Net revenue after a year.

## See Also

### Getting subscription dates

var renewalDate: Date?

The UNIX time, in milliseconds, that the most recent auto-renewable subscription purchase expires.

