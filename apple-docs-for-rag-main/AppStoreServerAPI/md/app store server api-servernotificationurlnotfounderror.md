

- App Store Server API
-  ServerNotificationURLNotFoundError 

Object

# ServerNotificationURLNotFoundError

An error that indicates the App Store server couldn’t find a notifications URL for your app in the environment.

App Store Server API 1.5+

``` source
object ServerNotificationURLNotFoundError
```

## Properties

`errorCode`

`number`

Value: `4040007`

`errorMessage`

`string`

For more information about configuring App Store Server Notifications in App Store Connect, see Enter a URL for App Store server notifications. Check that you’ve configured a server notifications URL for the production environment or sandbox enviroment, whichever you’re using.

Value: `No App Store Server Notification URL found for provided app. Check that a URL is configured in App Store Connect for this environment.`

## See Also

### Notification test and history errors

object InvalidEndDateError

An error that indicates the end date is invalid.

object InvalidNotificationTypeError

An error that indicates the notification type or subtype is invalid.

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

object StartDateAfterEndDateError

An error that indicates the end date precedes the start date, or the two dates are equal.

object StartDateTooFarInPastError

An error that indicates the start date is earlier than the earliest allowed date.

object TestNotificationNotFoundError

An error that indicates the test notification token is expired or the test notification status isn’t available.

