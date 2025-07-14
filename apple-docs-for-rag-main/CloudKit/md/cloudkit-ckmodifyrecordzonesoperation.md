

- CloudKit
-  CKModifyRecordZonesOperation 

Class

# CKModifyRecordZonesOperation

An operation that modifies one or more record zones.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKModifyRecordZonesOperation
```

## Mentioned in 

Encrypting User Data

Responding to Requests to Delete Data

## Overview

After you create one or more record zones, use this operation to save those zones to the database. You can also use the operation to delete record zones and their records.

If you assign a handler to the completionBlock property of the operation, CloudKit calls the handler after the operation executes and returns its results. Use the handler to perform housekeeping tasks for the operation, but don’t use it to process the results of the operation. The handler you provide should manage any failures of the operation, whether due to an error or an explicit cancellation.

## Topics

### Creating a Modify Zones Operation

convenience init(recordZonesToSave: [CKRecordZone]?, recordZoneIDsToDelete: [CKRecordZone.ID]?)

Creates an operation for modifying the specified record zones.

init()

Creates an empty modify record zones operation.

### Configuring the Modify Zones Operation

var recordZonesToSave: [CKRecordZone]?

The record zones to save to the database.

var recordZoneIDsToDelete: [CKRecordZone.ID]?

The IDs of the record zones to delete permanently from the database.

### Processing the Modify Zones Results

var modifyRecordZonesCompletionBlock: (([CKRecordZone]?, [CKRecordZone.ID]?, (any Error)?) -> Void)?

The closure to execute after CloudKit modifies all of the record zones.

Deprecated

### Instance Properties

var modifyRecordZonesResultBlock: ((Result&lt;Void, any Error>) -> Void)?

var perRecordZoneDeleteBlock: ((CKRecordZone.ID, Result&lt;Void, any Error>) -> Void)?

var perRecordZoneSaveBlock: ((CKRecordZone.ID, Result&lt;CKRecordZone, any Error>) -> Void)?

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

### Transactions

class CKModifyRecordsOperation

An operation that modifies one or more records.

