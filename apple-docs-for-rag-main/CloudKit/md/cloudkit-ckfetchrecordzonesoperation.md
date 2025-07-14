

- CloudKit
-  CKFetchRecordZonesOperation 

Class

# CKFetchRecordZonesOperation

An operation for retrieving record zones from a database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKFetchRecordZonesOperation
```

## Mentioned in 

Encrypting User Data

## Overview

Use this operation object to fetch record zones so that you can ascertain their capabilities.

If you assign a handler to the completionBlock property of the operation, CloudKit calls it after the operation executes and returns its results. You can use the handler to perform any housekeeping tasks that relate to the operation, but don’t use it to process the results of the operation. The handler you specify should manage any failures, whether due to an error or an explicit cancellation.

## Topics

### Initializing the Zone Fetch Operation

convenience init(recordZoneIDs: [CKRecordZone.ID])

Creates an operation for fetching the specified record zones.

init()

Creates an empty fetch zones operation.

### Getting All Record Zones

class func fetchAllRecordZonesOperation() -> Self

Returns an operation for fetching all record zones in the current database.

### Configuring a Zone Fetch Operation

var recordZoneIDs: [CKRecordZone.ID]?

The IDs of the record zones to retrieve.

### Processing Zone Fetch Results

var fetchRecordZonesCompletionBlock: (([CKRecordZone.ID : CKRecordZone]?, (any Error)?) -> Void)?

The closure to execute after CloudKit retrieves all of the record zones.

Deprecated

### Instance Properties

var fetchRecordZonesResultBlock: ((Result&lt;Void, any Error>) -> Void)?

var perRecordZoneResultBlock: ((CKRecordZone.ID, Result&lt;CKRecordZone, any Error>) -> Void)?

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

class CKFetchRecordsOperation

An operation for retrieving records from a database.

