

- App Store Server API
-  accountTenure 

Type

# accountTenure

The age of the customer’s account.

App Store Server API 1.0+

``` source
int32 accountTenure
```

## Possible Values 

`0`  

Account age is undeclared. Use this value to avoid providing information for this field.

`1`  

Account age is between 0–3 days.

`2`  

Account age is between 3–10 days.

`3`  

Account age is between 10–30 days.

`4`  

Account age is between 30–90 days.

`5`  

Account age is between 90–180 days.

`6`  

Account age is between 180–365 days.

`7`  

Account age is over 365 days.

## See Also

### Consumption Data Types

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

type playTime

A value that indicates the amount of time that the customer used the app.

type refundPreference

A value that indicates your preferred outcome for the refund request.

type sampleContentProvided

A Boolean value that indicates whether you provided, prior to its purchase, a free sample or trial of the content, or information about its functionality.

type userStatus

The status of a customer’s account within your app.

