

- CloudKit
-  CKPartialErrorsByItemIDKey 

Global Variable

# CKPartialErrorsByItemIDKey

The key to retrieve partial errors.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
let CKPartialErrorsByItemIDKey: String
```

## Discussion

The value of this key is a dictionary that maps an item ID to an error. The type of each ID depends on where the error occurs. For example, if you receive a partial error when modifying a record, the ID is an instance of CKRecord.ID that corresponds to the record that CloudKit can’t modify.

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

let CKErrorUserDidResetEncryptedDataKey: String

The key that determines whether CloudKit deletes a record zone because of a user action.

Record Changed Error Keys

Constants that represent conflicting records in a save operation.

