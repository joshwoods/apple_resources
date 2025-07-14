

- App Store Server API
-  SubscriptionExtensionIneligibleError 

Object

# SubscriptionExtensionIneligibleError

An error that indicates the subscription doesn’t qualify for a renewal-date extension due to its subscription state.

App Store Server API 1.1+

``` source
object SubscriptionExtensionIneligibleError
```

## Properties

`errorCode`

`number`

Value: `4030004`

`errorMessage`

`string`

Value: `Forbidden - subscription state ineligible for extension.`

## Discussion

This error applies to the Extend a Subscription Renewal Date endpoint.

Auto-renewable subscriptions in the following states aren’t eligible for renewal date extensions:

- Subscriptions in a free offer period

- Inactive subscriptions in a billing retry state

- Subscriptions in a grace period state with an expiration date in the past

- Subscriptions that have already received two renewal date extensions within the past 365 days

- Expired subscriptions

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

