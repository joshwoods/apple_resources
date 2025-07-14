

- App Store Server API
-  GeneralBadRequestError 

Object

# GeneralBadRequestError

An error that indicates an invalid request.

App Store Server API 1.1+

``` source
object GeneralBadRequestError
```

## Properties

`errorCode`

`number`

Value: `4000000`

`errorMessage`

`string`

Value: `Bad request.`

## Discussion

A bad request error typically occurs when the server receives a malformed request or a request that contains incorrect syntax.

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

object InvalidRequestRevisionError

An error that indicates an invalid request revision.

object InvalidRevokedError

An error that indicates the revoked parameter contains an invalid value.

object InvalidStatusError

An error that indicates the status parameter is invalid.

