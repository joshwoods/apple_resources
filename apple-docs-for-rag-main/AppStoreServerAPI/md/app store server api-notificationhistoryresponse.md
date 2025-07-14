

- App Store Server API
-  NotificationHistoryResponse 

Object

# NotificationHistoryResponse

A response that contains the App Store Server Notifications history for your app.

App Store Server API 1.5+

``` source
object NotificationHistoryResponse
```

## Properties

`notificationHistory`

`[`notificationHistoryResponseItem`]`

An array of App Store Server Notifications history records.

If you set onlyFailures to `true` in the NotificationHistoryRequest, this array contains only the notifications that failed to reach your server.

`hasMore`

hasMore

A Boolean value that indicates whether the App Store has more notification history records to send. If `hasMore` is `true`, use the `paginationToken` in the subsequent request to get more records. If `hasMore` is false, there are no more records available.

`paginationToken`

paginationToken

A pagination token that you provide to Get Notification History on a subsequent request to get the next page of responses.

## Mentioned in 

App Store Server API changelog

## Discussion

The Get Notification History endpoint returns this response. Notification history records contain the notifications that the App Store server attempted to send to your server’s App Store Server Notifications V2 endpoint.

The notification history response contains a maximum of 20 notification history records per response. If the history has more than 20 records, the hasMore value is `true`. Call Get Notification History again with `paginationToken` in the query to receive the next page of responses. When the App Store has no more records to send, the `hasMore` value is `false`.

Note

The notifications in the history records reflect the state of an in-app purchase at the time the App Store originally sent the notification, and may not reflect its current state. To get the current state of auto-renewable subscriptions, call the Get All Subscription Statuses endpoint. For all other in-app purchase types, call the Get Transaction History V1 endpoint.

## Topics

### Data types

type paginationToken

A pagination token that you return to the endpoint on a subsequent call to receive the next set of results.

type hasMore

A Boolean value indicating whether the App Store has more transaction data.

## See Also

### App Store Server Notifications history

Get Notification History

Get a list of notifications that the App Store server attempted to send to your server.

object NotificationHistoryRequest

The request body for notification history.

object notificationHistoryResponseItem

The App Store server notification history record, including the signed notification payload and the result of the server’s first send attempt.

