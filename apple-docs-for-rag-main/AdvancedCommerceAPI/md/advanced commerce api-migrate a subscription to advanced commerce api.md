

- Advanced Commerce API
-  Migrate a Subscription to Advanced Commerce API 

Web Service Endpoint

# Migrate a Subscription to Advanced Commerce API

Migrate a subscription that a customer purchased through In-App Purchase to a subscription you manage using the Advanced Commerce API.

Advanced Commerce API 1.0+

## URL

``` source
POST https://api.storekit.itunes.apple.com/advancedCommerce/v1/subscription/migrate/{transactionId}
```

## Sandbox URL

``` source
POST https://api.storekit-sandbox.itunes.apple.com/advancedCommerce/v1/subscription/migrate/{transactionId}
```

## Path Parameters

`transactionId`

`string`

 (Required) 

The transaction identifier of the auto-renewable subscription to migrate. Use the subscription’s original transaction ID or any subsequent transaction ID of a transaction related to the subscription.

## HTTP Body

SubscriptionMigrateRequest

The request body that contains the details for the migration.

Content-Type: application/json

## Response Codes

` 200 ``OK`

SubscriptionMigrateResponse

`OK`

Request succeeded.

Content-Type: application/json

` 400 ``Bad Request`

`(`RepeatedRequestReferenceIdError` | `NullRequestInfoError` | `NullTaxCodeError` | `NullItemsError` | `NullDescriptorsError` | `NullSKUError` | `NullDisplayNameError` | `NullDescriptionError` | `InvalidAppAccountTokenError` | `NullRequestReferenceIDError` | `InvalidRequestReferenceIDError` | `InvalidConsistencyTokenError` | `InvalidStorefrontError` | `SKULengthExceededError` | `DescriptionLengthExceededError` | `DisplayNameLengthExceededError` | `InvalidDisplayNameError` | `InvalidDescriptionError` | `InvalidProductError` | `InvalidSKUError` | `InvalidTaxProductCodeError` | `MismatchedStorefrontError` | `MissingPricingConfigForStorefrontError` | `OperationNotAllowedError` | `MalformedPayloadError` | `AtLeastOneItemError` | `NullTargetProductIDError` | `InvalidTargetProductIDError` | `SubscriptionAlreadyMigratedError` | `ItemLimitExceededError` | `PendingChangesMismatchError`)`

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid. For more information, see Authorizing API requests from your server.

` 403 ``Forbidden`

`(`SubscriptionDoesNotExistError` | `SubscriptionAlreadyExistsError` | `SubscriptionNotEligibleError` | `ProductNotOwnedError` | `InactiveACASubError` | `ProductNotEligibleError` | `StorefrontChangeError`)`

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

Advanced Commerce API changelog

Identifying rate limits for Advanced Commerce APIs

Authorizing API requests from your server

## Discussion

Note

You can use the Advanced Commerce API and the StoreKit In-App Purchase APIs in the same app. Both APIs use the App Store commerce system, including the same signed JWS transactions and JWS renewal info. For products that you offer using the In-App Purchase API, you set up product identifiers in App Store Connect. For products that you offer using the Advanced Commerce API, you host and manage your own catalog of SKUs and add product details dynamically at runtime.

## See Also

### Migration from the server

object SubscriptionMigrateRequest

The subscription details you provide to migrate a subscription from In-App Purchase to the Advanced Commerce API, such as descriptors, items, storefront, and more.

object SubscriptionMigrateResponse

A response that contains signed renewal and transaction information after a subscription successfully migrates to the Advanced Commerce API.

object SubscriptionMigrateItem

The SKU, description, and display name to use for a migrated subscription item.

object SubscriptionMigrateRenewalItem

The item information that replaces a migrated subscription item when the subscription renews.

object SubscriptionMigrateDescriptors

The description and display name of the subscription to migrate to that you manage.

