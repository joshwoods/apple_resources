

- App Store Server API
-  FamilySharedSubscriptionExtensionIneligibleError 

Object

# FamilySharedSubscriptionExtensionIneligibleError

An error that indicates a subscription isn’t directly eligible for a renewal date extension because the customer obtained it through Family Sharing.

App Store Server API 1.8+

``` source
object FamilySharedSubscriptionExtensionIneligibleError
```

## Properties

`errorCode`

`number`

Value: `4030007`

`errorMessage`

`string`

Value: `Subscriptions that users obtain through Family Sharing can't get a renewal date extension directly.`

## Mentioned in 

App Store Server API changelog

## Discussion

A request returns this error if you call the Extend a Subscription Renewal Date endpoint with an `originalTransactionId` that belongs to a subscription the user obtains through Family Sharing.

When the endpoint extends an eligible purchased subscription that supports Family Sharing, it automatically extends the family members’ subscriptions as well. However, the endpoint doesn’t support requests to extend a family member’s subscription directly.

## See Also

### Errors

object AccountNotFoundError

An error that indicates the App Store account wasn’t found.

object AppNotFoundError

An error that indicates the app wasn’t found.

object AppTransactionIdNotSupportedError

An error that indicates the endpoint doesn’t support an app transaction ID.

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

object InvalidStatusError

An error that indicates the status parameter is invalid.

