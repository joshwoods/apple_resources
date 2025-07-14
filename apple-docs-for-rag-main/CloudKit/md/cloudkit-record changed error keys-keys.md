

- CloudKit
-  Record Changed Error Keys 

API Collection

# Record Changed Error Keys

Constants that represent conflicting records in a save operation.

## Overview

If the version of a record on the server is newer than the version you try to save, the server returns a CKError.Code.serverRecordChanged error. The error’s userInfo dictionary contains the different versions of the conflicting records. Use these keys to retrieve the records, and to perform any resolution logic necessary to resolve the conflict.

## Topics

### Record Changed Error Keys

let CKRecordChangedErrorAncestorRecordKey: String

The key to retrieve the original version of the record.

let CKRecordChangedErrorClientRecordKey: String

The key to retrieve the local version of the record.

let CKRecordChangedErrorServerRecordKey: String

The key to retrieve the server’s version of the record.

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

let CKPartialErrorsByItemIDKey: String

The key to retrieve partial errors.

