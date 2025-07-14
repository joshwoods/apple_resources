

- App Store Server API
-  InvalidDeliveryStatusError 

Object

# InvalidDeliveryStatusError

An error that indicates the value in the delivery status field is invalid.

App Store Server API 1.9+

``` source
object InvalidDeliveryStatusError
```

## Properties

`errorCode`

`number`

Value: `4000036`

`errorMessage`

`string`

Value: `Invalid request. The delivery status field is invalid.`

## Mentioned in 

App Store Server API changelog

## Discussion

For valid `deliveryStatus` values in a ConsumptionRequest, see deliveryStatus.

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

object InvalidTransactionTypeNotSupportedError

An error that indicates the transaction identifier represents an unsupported In-App Purchase type.

object InvalidUserStatusError

An error that indicates the value in the user status field is invalid.

object InvalidTransactionNotConsumableError

An error that indicates the transaction identifier doesn’t represent a consumable In-App Purchase.

Deprecated

