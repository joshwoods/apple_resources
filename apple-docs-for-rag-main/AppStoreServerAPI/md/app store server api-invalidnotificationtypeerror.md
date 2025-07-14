

- App Store Server API
-  InvalidNotificationTypeError 

Object

# InvalidNotificationTypeError

An error that indicates the notification type or subtype is invalid.

App Store Server API 1.5+

``` source
object InvalidNotificationTypeError
```

## Properties

`errorCode`

`number`

Value: `4000018`

`errorMessage`

`string`

For a list of valid notification types and subtypes, see notificationType and subtype. If you provide both a notification type and subtype, ensure the two are a valid combination, as documented on subtype.

Value: `Invalid request. The notification type or subtype is invalid.`

## See Also

### Notification test and history errors

object InvalidEndDateError

An error that indicates the end date is invalid.

object InvalidPaginationTokenError

An error that indicates the pagination token is invalid.

object InvalidStartDateError

An error that indicates the start date is invalid.

object InvalidTestNotificationTokenError

An error that indicates the test notification token is invalid.

object InvalidInAppOwnershipTypeError

An error that indicates an invalid in-app ownership type parameter.

object InvalidProductIdError

An error that indicates the product ID parameter is invalid.

object InvalidProductTypeError

An error that indicates the product type parameter is invalid.

object InvalidSortError

An error that indicates the sort parameter is invalid.

object InvalidSubscriptionGroupIdentifierError

An error that indicates the subscription group identifier is invalid.

object MultipleFiltersSuppliedError

An error that indicates the request is invalid because it has too many applied constraints.

object PaginationTokenExpiredError

An error that indicates the pagination token expired.

object ServerNotificationURLNotFoundError

An error that indicates the App Store server couldn’t find a notifications URL for your app in the environment.

object StartDateAfterEndDateError

An error that indicates the end date precedes the start date, or the two dates are equal.

object StartDateTooFarInPastError

An error that indicates the start date is earlier than the earliest allowed date.

object TestNotificationNotFoundError

An error that indicates the test notification token is expired or the test notification status isn’t available.

