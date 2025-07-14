

- App Store Server API
-  userStatus 

Type

# userStatus

The status of a customer’s account within your app.

App Store Server API 1.0+

``` source
int32 userStatus
```

## Possible Values 

`0`  

Account status is undeclared. Use this value to avoid providing information for this field.

`1`  

The customer’s account is active.

`2`  

The customer’s account is suspended.

`3`  

The customer’s account is terminated.

`4`  

The customer’s account has limited access.

## Discussion

This user status represents the standing of a customer account in your app.

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

type playTime

A value that indicates the amount of time that the customer used the app.

type refundPreference

A value that indicates your preferred outcome for the refund request.

type sampleContentProvided

A Boolean value that indicates whether you provided, prior to its purchase, a free sample or trial of the content, or information about its functionality.

