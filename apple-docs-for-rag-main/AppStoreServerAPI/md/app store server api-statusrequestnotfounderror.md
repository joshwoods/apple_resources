

- App Store Server API
-  StatusRequestNotFoundError 

Object

# StatusRequestNotFoundError

An error that indicates the server didn’t find a subscription-renewal-date extension request for the request identifier and product identifier you provided.

App Store Server API 1.8+

``` source
object StatusRequestNotFoundError
```

## Properties

`errorCode`

`number`

Value: `4040009`

`errorMessage`

`string`

Value: `The server didn't find a subscription-renewal-date extension request for this requestIdentifier and productId combination.`

## Mentioned in 

App Store Server API changelog

## Discussion

This error applies to the Get Status of Subscription Renewal Date Extensions endpoint. Check that the `productId` and `requestIdentifier` parameters match the values associated with your request to the Extend Subscription Renewal Dates for All Active Subscribers endpoint.

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

