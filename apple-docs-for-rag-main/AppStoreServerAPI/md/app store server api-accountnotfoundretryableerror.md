

- App Store Server API
-  AccountNotFoundRetryableError 

Object

# AccountNotFoundRetryableError

An error response that indicates the App Store account wasn’t found, but you can try again.

App Store Server API 1.0+

``` source
object AccountNotFoundRetryableError
```

## Properties

`errorCode`

`number`

Value: `4040002`

`errorMessage`

`string`

Value: `Account not found. Please try again.`

## See Also

### Errors to retry

object AppNotFoundRetryableError

An error response that indicates the app wasn’t found, but you can try again.

object GeneralInternalRetryableError

An error response that indicates an unknown error occurred, but you can try again.

object OriginalTransactionIdNotFoundRetryableError

An error response that indicates the original transaction identifier wasn’t found, but you can try again.

