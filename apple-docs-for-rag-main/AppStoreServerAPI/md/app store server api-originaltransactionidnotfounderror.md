

- App Store Server API
-  OriginalTransactionIdNotFoundError 

Object

# OriginalTransactionIdNotFoundError

An error that indicates an original transaction identifier wasn’t found.

App Store Server API 1.0+

``` source
object OriginalTransactionIdNotFoundError
```

## Properties

`errorCode`

`number`

Value: `4040005`

`errorMessage`

`string`

Value: `Original transaction id not found.`

## Discussion

Don’t unlock the service or content associated with the transaction ID for the app bundle ID and environment that you indicate in the request unless you successfully resolve this error. To resolve this error, check your request to ensure that:

- The JSON Web Token (JWT) payload contains the bundle ID (`bid`) of your app that’s associated with the transaction ID. For more information, see Generating JSON Web Tokens for API requests.

- You’re making the request in the same environment, production or sandbox, that generated the transaction ID.

In rare cases, you might get this error for transaction IDs that previously returned data successfully. Don’t unlock the service or content for the app bundle ID and environment in the request if you’re unable to resolve this error using the steps above.

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

object InvalidRequestRevisionError

An error that indicates an invalid request revision.

object InvalidRevokedError

An error that indicates the revoked parameter contains an invalid value.

