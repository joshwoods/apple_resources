

- App Store Server API
-  GeneralInternalRetryableError 

Object

# GeneralInternalRetryableError

An error response that indicates an unknown error occurred, but you can try again.

App Store Server API 1.0+

``` source
object GeneralInternalRetryableError
```

## Properties

`errorCode`

`number`

Value: `5000001`

`errorMessage`

`string`

Value: `An unknown error occurred. Please try again.`

## See Also

### Errors to retry

object AccountNotFoundRetryableError

An error response that indicates the App Store account wasn’t found, but you can try again.

object AppNotFoundRetryableError

An error response that indicates the app wasn’t found, but you can try again.

object OriginalTransactionIdNotFoundRetryableError

An error response that indicates the original transaction identifier wasn’t found, but you can try again.

