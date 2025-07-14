

- CloudKit
-  CKFetchRecordsOperation 

Class

# CKFetchRecordsOperation

An operation for retrieving records from a database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKFetchRecordsOperation
```

## Mentioned in 

Encrypting User Data

## Overview

Use this operation to retrieve the entire contents of each record or only a subset of its contained values. As records become available, the operation object reports progress about the state of the operation to several different blocks, which you can use to process the results.

Fetching records is a common use of CloudKit, even if your app doesn’t cache record IDs locally. For example, when you fetch a record related to the current record through a CKRecord.Reference object, you use the ID in the reference to perform the fetch.

The handlers you assign to process the fetched records execute serially on an internal queue that the fetch operation manages. Your handlers must be capable of executing on a background thread, so any tasks that require access to the main thread must redirect accordingly.

In addition to data records, a fetch records operation can fetch the current user record. The fetchCurrentUserRecordOperation() method returns a specially configured operation object that retrieves the current user record. That record is a standard CKRecord object that has no content initially. You can add data to the user record and save it as necessary. Don’t store sensitive personal information, such as passwords, in the user record because other users of your app can access the discoverable user record in a public database. If you must store sensitive information about a user, do so in a separate record that is accessible only to that user.

If you assign a closure to the completionBlock property of the operation object, CloudKit calls it after the operation executes and returns its results. Use a closure to perform any housekeeping tasks for the operation, but don’t use it to process the results of the operation. The closure you specify should handle the failure of the operation to complete its task, whether due to an error or an explicit cancellation.

## Topics

### Creating a Record Fetch Operation

convenience init(recordIDs: [CKRecord.ID])

Creates a fetch operation for retrieving the records with the specified IDs.

init()

Creates an empty fetch operation.

### Getting the Current User Record

class func fetchCurrentUserRecordOperation() -> Self

Returns a fetch operation for retrieving the current user record.

### Configuring a Record Fetch Operation

var recordIDs: [CKRecord.ID]?

The record IDs of the records to fetch.

var desiredKeys: [CKRecord.FieldKey]?

The fields of the records to fetch.

### Processing Record Fetch Results

var perRecordProgressBlock: ((CKRecord.ID, Double) -> Void)?

The closure to execute with progress information for individual records.

var perRecordCompletionBlock: ((CKRecord?, CKRecord.ID?, (any Error)?) -> Void)?

The closure to execute when a record becomes available.

Deprecated

var fetchRecordsCompletionBlock: (([CKRecord.ID : CKRecord]?, (any Error)?) -> Void)?

The closure to execute after CloudKit retrieves all of the records.

Deprecated

### Instance Properties

var fetchRecordsResultBlock: ((Result&lt;Void, any Error>) -> Void)?

var perRecordResultBlock: ((CKRecord.ID, Result&lt;CKRecord, any Error>) -> Void)?

## Relationships

### Inherits From

- CKDatabaseOperation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Fetch Requests

class CKFetchRecordZonesOperation

An operation for retrieving record zones from a database.

