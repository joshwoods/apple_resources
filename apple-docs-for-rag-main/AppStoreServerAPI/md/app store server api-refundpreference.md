

- App Store Server API
-  refundPreference 

Type

# refundPreference

A value that indicates your preferred outcome for the refund request.

App Store Server API 1.11+

``` source
int32 refundPreference
```

## Possible Values 

`0`  

The refund preference is undeclared. Use this value to avoid providing information for this field.

`1`  

You prefer that Apple grants the refund.

`2`  

You prefer that Apple declines the refund.

`3`  

You have no preference whether Apple grants or declines the refund.

## Mentioned in 

App Store Server API changelog

## Discussion

Your refund preference is one of a variety of factors that the App Store uses to inform its refund decisions.

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

type sampleContentProvided

A Boolean value that indicates whether you provided, prior to its purchase, a free sample or trial of the content, or information about its functionality.

type userStatus

The status of a customer’s account within your app.

