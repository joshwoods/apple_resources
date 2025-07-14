

- App Store Server API
-  InvalidRequestRevisionError 

Object

# InvalidRequestRevisionError

An error that indicates an invalid request revision.

App Store Server API 1.0+

``` source
object InvalidRequestRevisionError
```

## Properties

`errorCode`

`number`

Value: `4000005`

`errorMessage`

`string`

Value: `Invalid request revision.`

## Discussion

This error applies to the revision query parameter of endpoints like Get Transaction History V1 and Get Refund History.

## See Also

### Errors

object AccountNotFoundError

An error that indicates the App Store account wasn’t found.

object AppNotFoundError

An error that indicates the app wasn’t found.

object AppTransactionIdNotSupportedError

An error that indicates the endpoint doesn’t support an app transaction ID.

object FamilySharedSubscriptionExtensionIneligibleError

An error that indicates a subscription isn’t directly eligible for a renewal date extension because the customer obtained it through Family Sharing.

object GeneralInternalError

An error that indicates a general internal error.

object GeneralBadRequestError

An error that indicates an invalid request.

object InvalidAppIdentifierError

An error that indicates an invalid app identifier.

object InvalidEmptyStorefrontCountryCodeListError

An error that indicates a required storefront country code is empty.

object InvalidExtendByDaysError

An error that indicates an invalid extend-by-days value.

object InvalidExtendReasonCodeError

An error that indicates an invalid reason code.

object InvalidOriginalTransactionIdError

An error that indicates an invalid original transaction identifier.

object InvalidRefundPreferenceError

An error that indicates an invalid refund preference code.

object InvalidRequestIdentifierError

An error that indicates an invalid request identifier.

object InvalidRevokedError

An error that indicates the revoked parameter contains an invalid value.

object InvalidStatusError

An error that indicates the status parameter is invalid.

