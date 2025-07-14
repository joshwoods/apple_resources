

- App Store Server API
-  InvalidEmptyStorefrontCountryCodeListError 

Object

# InvalidEmptyStorefrontCountryCodeListError

An error that indicates a required storefront country code is empty.

App Store Server API 1.7+

``` source
object InvalidEmptyStorefrontCountryCodeListError
```

## Properties

`errorCode`

`number`

Value: `4000027`

`errorMessage`

`string`

Value: `Invalid request. If provided, the list of storefront country codes must not be empty.`

## Discussion

This error applies to the Extend Subscription Renewal Dates for All Active Subscribers endpoint. If your request applies to all storefronts, omit the `storefrontCountryCodes` list from the MassExtendRenewalDateRequest object.

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

