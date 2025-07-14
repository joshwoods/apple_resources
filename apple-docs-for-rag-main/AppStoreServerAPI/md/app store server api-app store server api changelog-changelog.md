

- App Store Server API
-  App Store Server API changelog 

Article

# App Store Server API changelog

Learn about new features and updates in the App Store Server API.

## Overview

Use this changelog to learn about feature updates, deprecations, and removals for the App Store Server API.

### 1.15 - 2025/02/21

**New features**

- Updated the JWSRenewalInfoDecodedPayload and JWSTransactionDecodedPayload to include the new appTransactionId and offerPeriod fields.

- Updated the JWSRenewalInfoDecodedPayload to include the appAccountToken field.

- Added the AppTransactionIdNotSupportedError error object.

### 1.14 - 2025/01/17

- Added support for Advanced Commerce API.

### 1.13 — 2024/07/08

**New features**

- Updated the JWSRenewalInfoDecodedPayload to include the new eligibleWinBackOfferIds field.

- Added the win-back offer type in offerType.

### 1.12 — 2024/06/10

**New features**

- Added the endpoint Get Transaction History, which provides transaction history for all In-App Purchases, including consumable In-App Purchases in a finished state.

- Added the fields renewalPrice, currency and offerDiscountType to the JWSRenewalInfoDecodedPayload.

**Deprecations**

- The Get Transaction History V1 endpoint is deprecated. Use the new Get Transaction History endpoint instead.

### 1.11 — 2024/04/11

New features

- Added the refundPreference field to the ConsumptionRequest request body.

- Send Consumption Information added support for receiving information for auto-renewable subscriptions.

- Added the InvalidTransactionTypeNotSupportedError error object.

**Deprecations**

- The system no longer sends the InvalidTransactionNotConsumableError error object. It uses InvalidTransactionTypeNotSupportedError instead.

### 1.10.1 — 2024/03/12

- The type of the price field changed from `int32` to `int64`.

### Server update — 2024/02/29

**New features**

- The Get Notification History endpoint adds support for the new notification type for unreported external purchase tokens.

### 1.10 — 2023/10/26

New features

- Added the following new properties in the decoded transaction payload JWSTransactionDecodedPayload: price, currency, and offerDiscountType.

### 1.9 — 2023/09/27

New features

- Updated the error format of the Send Consumption Information endpoint to match that of other endpoints. The endpoint now returns a JSON body that can contain an error code.

- New error codes for the Send Consumption Information endpoint include: InvalidAccountTenureError, InvalidAppAccountTokenError, InvalidConsumptionStatusError, InvalidCustomerConsentedError, InvalidDeliveryStatusError, InvalidLifetimeDollarsPurchasedError, InvalidLifetimeDollarsRefundedError, InvalidPlatformError, InvalidPlayTimeError, InvalidSampleContentProvidedError, InvalidTransactionNotConsumableError, InvalidUserStatusError.

### 1.8 — 2023/06/05

New features

- Added a new endpoint Get Transaction Info with its response TransactionInfoResponse, which provides information about a single transaction.

- The Get Notification History endpoint adds a new filter parameter, onlyFailures. When you set it to `true`, the endpoint returns only the notifications that failed to reach the developer’s server.

- The following endpoints changed their path parameters from originalTransactionId to transactionId: Get All Subscription Statuses, Get Transaction History V1, Get Refund History, and Send Consumption Information. These endpoints now accept any transaction identifier, including original transaction identifiers.

- The Get Notification History endpoint now accepts a transactionId instead of requiring an original transaction identifier (originalTransactionId) in the NotificationHistoryRequest body.

- The Get Transaction History V1 endpoint adds a new filter parameter, `revoked`, that filters the response to return only revoked transactions or only nonrevoked transactions.

- The Get All Subscription Statuses endpoint adds a new filter parameter, `status`, that enables you to request subscriptions with the status values you specify.

- Added the storefront, storefrontId, and transactionReason fields to the JWSTransactionDecodedPayload object.

- Added the renewalDate field to the JWSRenewalInfoDecodedPayload object.

- Added the `sendAttempts` field to the CheckTestNotificationResponse and the notificationHistoryResponseItem of the NotificationHistoryResponse to provide information about all the send attempts for App Store Server Notifications.

- Added the error codes FamilySharedSubscriptionExtensionIneligibleError, StatusRequestNotFoundError, InvalidStatusError, InvalidRevokedError, InvalidTransactionIdError, TransactionIdNotFoundError, and RateLimitExceededError.

- All endpoints are subject to a rate limit and can return a RateLimitExceededError with an HTTP 429 error code. For more information, see Identifying rate limits.

**Deprecations**

- The `excludeRevoked` filter in Get Transaction History V1 is deprecated. Use the new `revoked` filter instead.

- The `firstSendAttemptResult` field is deprecated in the CheckTestNotificationResponse and notificationHistoryResponseItem objects. Use the first sendAttemptItem in the `sendAttempts` array instead.

### 1.7 — 2023/01/30

New features

- The new endpoint Extend Subscription Renewal Dates for All Active Subscribers takes a subscription product identifier and extends the renewal date for all eligible subscribers. It responds with MassExtendRenewalDateResponse. For more information, see Extending the renewal date for auto-renewable subscriptions. For information about new App Store server notifications related to this endpoint, see the App Store Server Notifications changelog.

- The new endpoint Get Status of Subscription Renewal Date Extensions checks the status of a subscription-renewal-date extension, and responds with the MassExtendRenewalDateStatusResponse.

### 1.6 — 2022/08/08

New features

- The new version 2 endpoint Get Refund History returns a paginated list of refunded transactions in the RefundHistoryResponse.

Deprecations

- The endpoint Get Refund History V1 and its response RefundLookupResponse are deprecated.

- In `firstSendAttemptResult`, the `SSL_ISSUE` value is deprecated and replaced with `TLS_ISSUE`.

### 1.5 — 2022/06/06

New features

- The API has two new endpoints to support testing how your server receives App Store Server Notifications. The endpoints are: Request a Test Notification and Get Test Notification Status.

- The API adds the new Get Notification History endpoint.

- The Get Transaction History V1 endpoint is enhanced with new parameters to support filtering and sorting functionality.

- The JWSRenewalInfoDecodedPayload now includes the recentSubscriptionStartDate field.

### 1.4

This version doesn’t contain any public changes.

### 1.3

This version doesn’t contain any public changes.

### Server update — 2022/03/17

Removals

- The JWSDecodedHeader object no longer includes the `kid` field.

### 1.2 — 2022/02/24

New features

- The JWSTransactionDecodedPayload and JWSRenewalInfoDecodedPayload objects now include the environment field.

### Server update — 2022/02/23

- The Get Refund History V1 endpoint now returns a maximum of 50 refunded transactions.

### 1.1 — 2022/10/21

New features

- The API adds three endpoints: Look Up Order ID, Get Refund History V1, and Extend a Subscription Renewal Date.

### Server update — 2021/09/20

The API is now available in the production environment, using the following base URL:

```
https://api.storekit.itunes.apple.com/inApps/
```

### 1.0b1 — 2021/06/07

Initial version of the App Store Server API.

New features

- This API has three endpoints, available in the sandbox environment: Get Transaction History V1, Send Consumption Information, and Get All Subscription Statuses.

## See Also

### Essentials

Simplifying your implementation by using the App Store Server Library

Use Apple’s open source library to create JSON Web Tokens (JWT) to authorize your calls, verify transactions, extract transaction identifiers from receipts, and more.

Creating API keys to authorize API requests

Create API keys you use to sign JSON Web Tokens and authorize API requests.

Generating JSON Web Tokens for API requests

Create JSON Web Tokens signed with your private key to authorize requests for App Store Server API and External Purchase Server API.

Identifying rate limits

Recognize the rate limits that apply to App Store Server API endpoints and handle them in your code.

