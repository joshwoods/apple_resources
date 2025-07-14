

- App Store Server API
-  InvalidAccountTenureError 

Object

# InvalidAccountTenureError

An error that indicates the value of the account tenure field is invalid.

App Store Server API 1.9+

``` source
object InvalidAccountTenureError
```

## Properties

`errorCode`

`number`

Value: `4000032`

`errorMessage`

`string`

Value: `Invalid request. The account tenure field is invalid.`

## Mentioned in 

App Store Server API changelog

## Discussion

For more information about `accountTenure` values in a ConsumptionRequest, see accountTenure.

## See Also

### Consumption request errors

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

object InvalidTransactionTypeNotSupportedError

An error that indicates the transaction identifier represents an unsupported In-App Purchase type.

object InvalidUserStatusError

An error that indicates the value in the user status field is invalid.

object InvalidTransactionNotConsumableError

An error that indicates the transaction identifier doesn’t represent a consumable In-App Purchase.

Deprecated

