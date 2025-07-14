

- App Store Server API
-  playTime 

Type

# playTime

A value that indicates the amount of time that the customer used the app.

App Store Server API 1.0+

``` source
int32 playTime
```

## Possible Values 

`0`  

The engagement time is undeclared. Use this value to avoid providing information for this field.

`1`  

The engagement time is between 0–5 minutes.

`2`  

The engagement time is between 5–60 minutes.

`3`  

The engagement time is between 1–6 hours.

`4`  

The engagement time is between 6–24 hours.

`5`  

The engagement time is between 1–4 days.

`6`  

The engagement time is between 4–16 days.

`7`  

The engagement time is over 16 days.

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

type deliveryStatus

A value that indicates whether the app successfully delivered an in-app purchase that works properly.

type lifetimeDollarsPurchased

A value that indicates the dollar amount of in-app purchases the customer has made in your app, since purchasing the app, across all platforms.

type lifetimeDollarsRefunded

A value that indicates the dollar amount of refunds the customer has received in your app, since purchasing the app, across all platforms.

type platform

The platform on which the customer consumed the in-app purchase.

type refundPreference

A value that indicates your preferred outcome for the refund request.

type sampleContentProvided

A Boolean value that indicates whether you provided, prior to its purchase, a free sample or trial of the content, or information about its functionality.

type userStatus

The status of a customer’s account within your app.

