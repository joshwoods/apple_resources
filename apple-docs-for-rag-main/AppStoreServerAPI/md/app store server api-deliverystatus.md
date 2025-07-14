

- App Store Server API
-  deliveryStatus 

Type

# deliveryStatus

A value that indicates whether the app successfully delivered an in-app purchase that works properly.

App Store Server API 1.0+

``` source
int32 deliveryStatus
```

## Possible Values 

`0`  

The app delivered the consumable in-app purchase and it’s working properly.

`1`  

The app didn’t deliver the consumable in-app purchase due to a quality issue.

`2`  

The app delivered the wrong item.

`3`  

The app didn’t deliver the consumable in-app purchase due to a server outage.

`4`  

The app didn’t deliver the consumable in-app purchase due to an in-game currency change.

`5`  

The app didn’t deliver the consumable in-app purchase for other reasons.

## See Also

### Consumption Data Types

type accountTenure

The age of the customer’s account.

type appAccountToken

The UUID that an app optionally generates to map a customer’s In-App Purchase with its resulting App Store transaction.

type consumptionStatus

A value that indicates the extent to which the customer consumed the in-app purchase.

type customerConsented

A Boolean value that indicates whether the customer consented to provide consumption data to the App Store.

type lifetimeDollarsPurchased

A value that indicates the dollar amount of in-app purchases the customer has made in your app, since purchasing the app, across all platforms.

type lifetimeDollarsRefunded

A value that indicates the dollar amount of refunds the customer has received in your app, since purchasing the app, across all platforms.

type platform

The platform on which the customer consumed the in-app purchase.

type playTime

A value that indicates the amount of time that the customer used the app.

type refundPreference

A value that indicates your preferred outcome for the refund request.

type sampleContentProvided

A Boolean value that indicates whether you provided, prior to its purchase, a free sample or trial of the content, or information about its functionality.

type userStatus

The status of a customer’s account within your app.

