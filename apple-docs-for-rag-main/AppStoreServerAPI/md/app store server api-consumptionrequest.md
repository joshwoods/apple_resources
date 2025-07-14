

- App Store Server API
-  ConsumptionRequest 

Object

# ConsumptionRequest

The request body containing consumption information.

App Store Server API 1.0+

``` source
object ConsumptionRequest
```

## Properties

`accountTenure`

accountTenure

**(Required)** The age of the customer’s account.

`appAccountToken`

appAccountToken

**(Required)** The UUID of the in-app user account that completed the in-app purchase transaction.

`consumptionStatus`

consumptionStatus

**(Required)** A value that indicates the extent to which the customer consumed the in-app purchase.

`customerConsented`

customerConsented

**(Required)** A Boolean value of `true` or `false` that indicates whether the customer consented to provide consumption data.

Note: The App Store server rejects requests that have a customerConsented value other than `true` by returning an `HTTP 400` error with an `InvalidCustomerConsentError`.

`deliveryStatus`

deliveryStatus

**(Required)** A value that indicates whether the app successfully delivered an in-app purchase that works properly.

`lifetimeDollarsPurchased`

lifetimeDollarsPurchased

**(Required)** A value that indicates the total amount, in USD, of in-app purchases the customer has made in your app, across all platforms.

`lifetimeDollarsRefunded`

lifetimeDollarsRefunded

**(Required)** A value that indicates the total amount, in USD, of refunds the customer has received, in your app, across all platforms.

`platform`

platform

**(Required)** A value that indicates the platform on which the customer consumed the in-app purchase.

`playTime`

playTime

**(Required)** A value that indicates the amount of time that the customer used the app.

`refundPreference`

refundPreference

A value that indicates your preference, based on your operational logic, as to whether Apple should grant the refund.

`sampleContentProvided`

sampleContentProvided

**(Required)** A Boolean value of `true` or `false` that indicates whether you provided, prior to its purchase, a free sample or trial of the content, or information about its functionality.

`userStatus`

userStatus

**(Required)** The status of the customer’s account.

## Mentioned in 

App Store Server API changelog

## Discussion

Use `ConsumptionRequest` to provide information about the customer’s consumable in-app purchase or auto-renewable subscription when you call the Send Consumption Information endpoint.

To create a valid request and avoid an `HTTP 400 Bad Request` error, ConsumptionRequest must contain all the required fields with proper data types and valid values. However, you can choose whether or not to provide information for most fields. Most fields have a valid option if you choose not to provide the information.

Note

Use the field value for *undeclared*, where available, if you choose not to provide information.

For example, if you choose not to provide information for the accountTenure field, set accountTenure to `0`. If you choose not to provide information for the appAccountToken field, set its value to an empty string. Refer to each field’s documentation for the list of valid values, including the undeclared value where available.

The App Store server rejects requests that have a customerConsented value other than `true` by returning an `HTTP 400` error with an `InvalidCustomerConsentError`.

## Topics

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

type userStatus

The status of a customer’s account within your app.

## See Also

### Consumption information

Send Consumption Information

Send consumption information about a consumable in-app purchase or auto-renewable subscription to the App Store after your server receives a consumption request notification.

