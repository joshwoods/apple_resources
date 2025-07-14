

- App Store Server API
-  InvalidTransactionTypeNotSupportedError 

Object

# InvalidTransactionTypeNotSupportedError

An error that indicates the transaction identifier represents an unsupported In-App Purchase type.

App Store Server API 1.11+

``` source
object InvalidTransactionTypeNotSupportedError
```

## Properties

`errorCode`

`number`

Value: `4000047`

`errorMessage`

`string`

Value: `Invalid request. The transaction id doesn't represent a supported in-app purchase type.`

## Mentioned in 

App Store Server API changelog

## Discussion

The Send Consumption Information endpoint returns this error if the `transactionId` doesn’t represent a supported in-app purchase. Be sure to provide the same `transactionId` that you receive to your App Store Server Notifications V2 endpoint in a notification with a `CONSUMPTION_REQUEST` notificationType.

## See Also

### Consumption request errors

object InvalidAccountTenureError

An error that indicates the value of the account tenure field is invalid.

object InvalidAppAccountTokenError

An error that indicates the value of the app account token field is invalid.

object InvalidConsumptionStatusError

An error that indicates the value of the consumption status field is invalid.

object InvalidCustomerConsentedError

An error that indicates the customer consented field is invalid or doesn’t indicate that the customer consented.

object InvalidDeliveryStatusError

An error that indicates the value in the delivery status field is invalid.

object InvalidLifetimeDollarsPurchasedError

An error that indicates the value in the lifetime dollars purchased field is invalid.

object InvalidLifetimeDollarsRefundedError

An error that indicates the value in the lifetime dollars refunded field is invalid.

object InvalidPlatformError

An error that indicates the value in the platform field is invalid.

object InvalidPlayTimeError

An error that indicates the value in the playtime field is invalid.

object InvalidSampleContentProvidedError

An error that indicates the value in the sample content provided field is invalid.

object InvalidUserStatusError

An error that indicates the value in the user status field is invalid.

object InvalidTransactionNotConsumableError

An error that indicates the transaction identifier doesn’t represent a consumable In-App Purchase.

Deprecated

