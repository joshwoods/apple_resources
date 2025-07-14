

- App Store Server API
-  InvalidRequestIdentifierError 

Object

# InvalidRequestIdentifierError

An error that indicates an invalid request identifier.

App Store Server API 1.1+

``` source
object InvalidRequestIdentifierError
```

## Properties

`errorCode`

`number`

Value: `4000011`

`errorMessage`

`string`

Value: `Invalid request identifier.`

## Discussion

This error applies to the requestIdentifier you provide in the Extend a Subscription Renewal Date, Extend Subscription Renewal Dates for All Active Subscribers, and Get Status of Subscription Renewal Date Extensions endpoints.

For the Extend Subscription Renewal Dates for All Active Subscribers and Get Status of Subscription Renewal Date Extensions endpoints, the requestIdentifier needs to be a `UUID`.

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

object InvalidRequestRevisionError

An error that indicates an invalid request revision.

object InvalidRevokedError

An error that indicates the revoked parameter contains an invalid value.

object InvalidStatusError

An error that indicates the status parameter is invalid.

