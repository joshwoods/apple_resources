

- App Store Server API
-  lifetimeDollarsRefunded 

Type

# lifetimeDollarsRefunded

A value that indicates the dollar amount of refunds the customer has received in your app, since purchasing the app, across all platforms.

App Store Server API 1.0+

``` source
int32 lifetimeDollarsRefunded
```

## Possible Values 

`0`  

Lifetime refund amount is undeclared. Use this value to avoid providing information for this field.

`1`  

Lifetime refund amount is 0 USD.

`2`  

Lifetime refund amount is between 0.01–49.99 USD.

`3`  

Lifetime refund amount is between 50–99.99 USD.

`4`  

Lifetime refund amount is between 100–499.99 USD.

`5`  

Lifetime refund amount is between 500–999.99 USD.

`6`  

Lifetime refund amount is between 1000–1999.99 USD.

`7`  

Lifetime refund amount is over 2000 USD.

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

