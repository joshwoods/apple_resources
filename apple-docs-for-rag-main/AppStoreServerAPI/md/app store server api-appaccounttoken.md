

- App Store Server API
-  appAccountToken 

Type

# appAccountToken

The UUID that an app optionally generates to map a customer’s In-App Purchase with its resulting App Store transaction.

App Store Server API 1.0+

``` source
uuid appAccountToken
```

## Mentioned in 

App Store Server API changelog

## Discussion

When a customer initiates an in-app purchase, you can optionally generate an appAccountToken(_:) and send it to the App Store. If you use the Original API for In-App Purchase, you may provide a UUID in the applicationUsername property. The App Store returns the same UUID in appAccountToken in the transaction information after the customer completes the purchase.

The ConsumptionRequest response body requires that you set the `appAccountToken` value to a valid value of either a UUID or an empty string. Set the `appAccountToken` value to the value you received in the `CONSUMPTION_REQUEST` notification, or, if you choose not to provide this information, set the value to an empty string.

If you receive a `CONSUMPTION_REQUEST` notification for a transaction, find its associated `appAccountToken` value as follows:

- If you receive App Store Server Notifications version 2, the `appAccountToken` value is in JWSTransactionDecodedPayload.

- If you receive App Store Server Notifications version 1, the `appAccountToken` value is in unified_receipt.Latest_receipt_info.

The `appAccountToken` value may be an empty string if your app doesn’t use app account tokens.

For more information about App Store Server Notifications versions, see App Store Server Notifications changelog.

## See Also

### Consumption Data Types

type accountTenure

The age of the customer’s account.

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

