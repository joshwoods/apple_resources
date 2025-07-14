

- CloudKit
-  CKErrorUserDidResetEncryptedDataKey 

Global Variable

# CKErrorUserDidResetEncryptedDataKey

The key that determines whether CloudKit deletes a record zone because of a user action.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let CKErrorUserDidResetEncryptedDataKey: String
```

## Mentioned in 

Encrypting User Data

## Discussion

An NSNumber that represents a Boolean value you use to determine whether a user action causes CloudKit to delete a record zone. CloudKit adds this key to the error’s `userInfo` dictionary when the error code is CKError.Code.zoneNotFound.

## See Also

### Errors

let CKErrorDomain: String

The error domain for CloudKit errors.

struct CKError

A type that describes a CloudKit error.

enum Code

The error codes that CloudKit returns.

let CKErrorRetryAfterKey: String

The key to retrieve the number of seconds to wait before you retry a request.

let CKPartialErrorsByItemIDKey: String

The key to retrieve partial errors.

Record Changed Error Keys

Constants that represent conflicting records in a save operation.

