

- App Store Server API
-  consumptionStatus 

Type

# consumptionStatus

A value that indicates the extent to which the customer consumed the in-app purchase.

App Store Server API 1.0+

``` source
int32 consumptionStatus
```

## Possible Values 

`0`  

The consumption status is undeclared. Use this value to avoid providing information for this field.

`1`  

The in-app purchase is not consumed.

`2`  

The in-app purchase is partially consumed.

`3`  

The in-app purchase is fully consumed.

## Discussion

Some examples of consumption status include the following scenarios:

- Scenario 1: A user purchases a “bag of 100 coins” in your app and spends all 100 coins. The in-app purchase is considered fully consumed.

- Scenario 2: If your app has an exchange platform that has bartering, or if your app transferred an in-app purchase from one account to another user’s account, the in-app purchase is considered fully consumed.

## See Also

### Consumption Data Types

type accountTenure

The age of the customer’s account.

type appAccountToken

The UUID that an app optionally generates to map a customer’s In-App Purchase with its resulting App Store transaction.

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

