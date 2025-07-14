

- App Store Server API
-  Get Notification History 

Web Service Endpoint

# Get Notification History

Get a list of notifications that the App Store server attempted to send to your server.

App Store Server API 1.5+

## URL

``` source
POST https://api.storekit.itunes.apple.com/inApps/v1/notifications/history
```

## Sandbox URL

``` source
POST https://api.storekit-sandbox.itunes.apple.com/inApps/v1/notifications/history
```

## Query Parameters

`paginationToken`

paginationToken

An optional token you use to get the next set of up to 20 notification history records. All responses that have more records available include a `paginationToken`.

Note: Omit this parameter the first time you call this endpoint.

## HTTP Body

NotificationHistoryRequest

The request body that includes the start and end dates, and optional query constraints.

Content-Type: application/json

## Response Codes

` 200 ``OK`

NotificationHistoryResponse

`OK`

Request succeeded.

Content-Type: application/json

` 400 ``Bad Request`

`(`InvalidTransactionIdError` | `PaginationTokenExpiredError` | `InvalidPaginationTokenError` | `InvalidStartDateError` | `InvalidEndDateError` | `StartDateAfterEndDateError` | `StartDateTooFarInPastError` | `InvalidNotificationTypeError` | `MultipleFiltersSuppliedError`)`

`Bad Request`

Invalid request.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid. For more information, see Generating JSON Web Tokens for API requests.

` 404 ``Not Found`

`(`TransactionIdNotFoundError` | `AccountNotFoundError`)`

`Not Found`

Content-Type: application/json

` 429 `

RateLimitExceededError

The request exceeded the rate limit.

Content-Type: application/json

` 500 ``Internal Server Error`

`(`GeneralInternalError` | `GeneralInternalRetryableError`)`

`Internal Server Error`

Server error. Try again later.

Content-Type: application/json

## Mentioned in 

App Store Server API changelog

Identifying rate limits

## Discussion

Call this endpoint to get a paginated list of the version 2 App Store Server Notifications that the App Store attempted to send to your server’s App Store Server Notifications V2 endpoint in a specified timespan. Choose a start date for the timespan that’s within the past 180 days.

You can further limit the request by specifying a `notificationType` or `notificationSubtype` in the NotificationHistoryRequest object. Alternatively, to get the notification history for a single user, provide a `transactionId`. The response, NotificationHistoryResponse, contains the full contents of the original notifications.

Each time you call this endpoint, it returns a maximum of 20 notification history records. If the hasMore field in the NotificationHistoryResponse is `true`, use the paginationToken from the response in your subsequent request to get the next set of records. Use the same NotificationHistoryRequest body on subsequent requests.

This endpoint is available in the production and sandbox environments. For more information about configuring App Store Server Notifications, see Enabling App Store Server Notifications and Enter a URL for App Store server notifications.

Note

For notifications that relate to in-app purchases, the history records reflect the state of an in-app purchase at the time the App Store originally sent the notification, and may not reflect its current state. To get the current state of auto-renewable subscriptions, call the Get All Subscription Statuses endpoint. For all other in-app purchase types, call the Get Transaction History V1 endpoint.

## See Also

### App Store Server Notifications history

object NotificationHistoryRequest

The request body for notification history.

object NotificationHistoryResponse

A response that contains the App Store Server Notifications history for your app.

object notificationHistoryResponseItem

The App Store server notification history record, including the signed notification payload and the result of the server’s first send attempt.

