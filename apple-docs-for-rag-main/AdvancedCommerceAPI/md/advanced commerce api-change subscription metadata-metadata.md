

- Advanced Commerce API
-  Change Subscription Metadata 

Web Service Endpoint

# Change Subscription Metadata

Update the SKU, display name, and description associated with a subscription, without affecting the subscription’s billing or its service.

Advanced Commerce API 1.0+

## URL

``` source
POST https://api.storekit.itunes.apple.com/advancedCommerce/v1/subscription/changeMetadata/{transactionId}
```

## Sandbox URL

``` source
POST https://api.storekit-sandbox.itunes.apple.com/advancedCommerce/v1/subscription/changeMetadata/{transactionId}
```

## Path Parameters

`transactionId`

`string`

 (Required) 

The transaction identifier of the auto-renewable subscription to get changes to its metadata. Use the subscription’s original transaction ID or any subsequent transaction ID of a transaction related to the subscription.

## HTTP Body

SubscriptionChangeMetadataRequest

The request body that contains the metadata changes.

Content-Type: application/json

## Response Codes

` 200 ``OK`

SubscriptionChangeMetadataResponse

`OK`

Request succeeded.

Content-Type: application/json

` 400 ``Bad Request`

`(`RepeatedRequestReferenceIdError` | `NullRequestInfoError` | `NullEffectiveError` | `InvalidAppAccountTokenError` | `NullRequestReferenceIDError` | `InvalidRequestReferenceIDError` | `InvalidConsistencyTokenError` | `InvalidStorefrontError` | `SKULengthExceededError` | `DescriptionLengthExceededError` | `DisplayNameLengthExceededError` | `InvalidProductChangesError` | `InvalidDisplayNameError` | `InvalidDescriptionError` | `InvalidProductError` | `InvalidSKUError` | `InvalidTaxProductCodeError` | `MismatchedStorefrontError` | `MismatchedStorefrontError` | `OperationNotAllowedError` | `MalformedPayloadError` | `AtLeastOneItemError` | `AtLeastOneOfDisplayNameOrDescriptionError`)`

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid. For more information, see Authorizing API requests from your server.

` 403 ``Forbidden`

`(`SubscriptionDoesNotExistError` | `SubscriptionNotEligibleError` | `ProductNotOwnedError` | `InactiveACASubError` | `ProductNotEligibleError`)`

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

`(`TransactionIdNotFoundError` | `ProductNotFoundError`)`

`Not Found`

Content-Type: application/json

` 429 `

RateLimitExceededError

The request exceeded the rate limit. For more information, see Identifying rate limits for Advanced Commerce APIs.

Content-Type: application/json

` 500 ``Internal Server Error`

`(`GeneralInternalError` | `GeneralInternalRetryableError`)`

`Internal Server Error`

Server error. Try again later.

Content-Type: application/json

## Mentioned in 

Identifying rate limits for Advanced Commerce APIs

Authorizing API requests from your server

Advanced Commerce API changelog

## Discussion

Use this endpoint to update the display name and description of an auto-renewable subscription. Calling this endpoint doesn’t change the price, billing details, or the service. For example, you can call `Change Subscription Metadata` if a subscription’s display name changes due to a change in its branding.

Don’t call this endpoint if a customer is changing subscriptions to receive a different service, such as upgrading, downgrading, or cross-grading. For such changes, use SubscriptionModifyInAppRequest.

## See Also

### Subscription metadata changes from the server

object SubscriptionChangeMetadataRequest

The request body you provide to change the metadata of a subscription.

object SubscriptionChangeMetadataResponse

The response body for a successful subscription metadata change.

object SubscriptionChangeMetadataDescriptors

The subscription metadata to change, specifically the description and display name.

object SubscriptionChangeMetadataItem

The metadata to change for an item, specifically its SKU, description, and display name.

