

- CloudKit
-  CKErrorRetryAfterKey 

Global Variable

# CKErrorRetryAfterKey

The key to retrieve the number of seconds to wait before you retry a request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
let CKErrorRetryAfterKey: String
```

## Discussion

An NSNumber that contains the number of seconds until you can retry a request. CloudKit adds this key to the error’s userInfo dictionary when the error code is CKError.Code.serviceUnavailable or CKError.Code.requestRateLimited.

## See Also

### Errors

let CKErrorDomain: String

The error domain for CloudKit errors.

struct CKError

A type that describes a CloudKit error.

enum Code

The error codes that CloudKit returns.

let CKErrorUserDidResetEncryptedDataKey: String

The key that determines whether CloudKit deletes a record zone because of a user action.

let CKPartialErrorsByItemIDKey: String

The key to retrieve partial errors.

Record Changed Error Keys

Constants that represent conflicting records in a save operation.

