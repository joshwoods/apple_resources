

- App Store Server API
-  recentSubscriptionStartDate 

Type

# recentSubscriptionStartDate

The earliest start date of a subscription in a series of auto-renewable subscription purchases that ignores all lapses of paid service shorter than 60 days.

App Store Server API 1.5+

``` source
timestamp recentSubscriptionStartDate
```

## Mentioned in 

App Store Server API changelog

## Discussion

The recent subscription start date is in UNIX time, in milliseconds.

Use the recentSubscriptionStartDate to identify the earliest start date of a subscription in a series of auto-renewable subscription purchases that the customer maintained continuously, or that has one or more gaps of less than 60 days each.

The App Store calculates the recentSubscriptionStartDate by finding the start date of the most recent auto-renewable subscription purchase that’s preceded by a gap in paid service of more than 60 days in the production environment, or 10 minutes in the sandbox environment. The start date includes any free trials or promotional purchases. If no such gap exists — for example, if the user has only ever purchased one subscription — the recentSubscriptionStartDate is the same as the subscription’s originalPurchaseDate.

The recentSubscriptionStartDate calculation counts a grace period or a billing retry state as a gap in the paid service.

Important

Don’t use the recentSubscriptionStartDate date to calculate days of paid service. For more information about paid days of service, see Net revenue after a year.

This date applies to active or expired subscriptions. For example, if a subscriber purchases an auto-renewable subscription on June 1, 2022 and lets it expire on December 31, 2022, the App Store determines the recent subscription start date as follows:

- Initially, the recentSubscriptionStartDate is the same as the originalPurchaseDate: June 1, 2022.

- If the customer purchases the subscription again on February 1, 2023, less than 60 days after the initial subscription expired, the recentSubscriptionStartDate remains June 1, 2022.

- If the customer purchases the subscription again on April 1, 2023, more than 60 days after the first subscription expired, the App Store updates the recentSubscriptionStartDate to April 1, 2023.

## See Also

### Purchase dates

type originalPurchaseDate

The purchase date of the transaction associated with the original transaction identifier.

type purchaseDate

The time that the App Store charged the customer’s account for an In-App Purchase, a restored In-App Purchase, a subscription, or a subscription renewal after a lapse.

