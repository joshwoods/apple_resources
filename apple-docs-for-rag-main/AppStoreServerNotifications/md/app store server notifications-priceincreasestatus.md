

- App Store Server Notifications
-  priceIncreaseStatus 

Type

# priceIncreaseStatus

The status that indicates whether an auto-renewable subscription is subject to a price increase.

App Store Server Notifications 2.0+

``` source
int32 priceIncreaseStatus
```

## Possible Values 

`0`  

The customer hasn’t yet responded to an auto-renewable subscription price increase that requires customer consent.

`1`  

The customer consented to an auto-renewable subscription price increase that requires customer consent, or the App Store has notified the customer of an auto-renewable subscription price increase that doesn’t require consent.

## Discussion

For more information about managing prices, see Managing Prices and Manage pricing for auto-renewable subscriptions.

