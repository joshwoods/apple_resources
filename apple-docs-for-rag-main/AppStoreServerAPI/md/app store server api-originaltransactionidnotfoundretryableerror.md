

- App Store Server API
-  OriginalTransactionIdNotFoundRetryableError 

Object

# OriginalTransactionIdNotFoundRetryableError

An error response that indicates the original transaction identifier wasn’t found, but you can try again.

App Store Server API 1.0+

``` source
object OriginalTransactionIdNotFoundRetryableError
```

## Properties

`errorCode`

`number`

Value: `4040006`

`errorMessage`

`string`

Value: `Original transaction id not found. Please try again.`

## See Also

### Errors to retry

object AccountNotFoundRetryableError

An error response that indicates the App Store account wasn’t found, but you can try again.

object AppNotFoundRetryableError

An error response that indicates the app wasn’t found, but you can try again.

object GeneralInternalRetryableError

An error response that indicates an unknown error occurred, but you can try again.

