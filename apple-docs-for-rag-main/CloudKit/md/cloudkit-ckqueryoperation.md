

- CloudKit
-  CKQueryOperation 

Class

# CKQueryOperation

An operation for executing queries in a database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKQueryOperation
```

## Overview

A `CKQueryOperation` object is a concrete operation that you can use to execute queries. A query operation applies query parameters to the specified database and record zone, delivering any matching records asynchronously to the handlers that you provide.

To perform a new search:

1.  Initialize a `CKQueryOperation` object with a CKQuery object that contains the search criteria and sorting information for the records you want.

2.  Assign a handler to the queryCompletionBlock property so that you can process the results and execute the operation.

If the search yields many records, the operation object may deliver a portion of the total results to your blocks immediately, along with a cursor for obtaining the remaining records. Use the cursor to initialize and execute a separate `CKQueryOperation` instance when you’re ready to process the next batch of results. 3. Optionally, configure the results by specifying values for the resultsLimit and desiredKeys properties. 4. Pass the query operation object to the add(_:) method of the target database to execute the operation.

CloudKit restricts queries to the records in a single record zone. For new queries, you specify the zone when you initialize the query operation object. For cursor-based queries, the cursor contains the zone information. To search for records in multiple zones, you must create a separate `CKQueryOperation` object for each zone you want to search, although you can initialize each of them with the same CKQuery object.

If you assign a handler to the operation’s completionBlock property, the operation calls it after it executes and returns any results. Use a handler to perform housekeeping tasks for the operation, but don’t use it to process the results of the operation. The handler you provide should manage any failures, whether due to an error or an explicit cancellation.

## Topics

### Creating a Query Operation

convenience init(query: CKQuery)

Creates an operation that searches for records in the specified record zone.

convenience init(cursor: CKQueryOperation.Cursor)

Creates an operation with additional results from a previous search.

init()

Creates an empty query operation.

### Configuring the Query Operation

var query: CKQuery?

The query for the search.

var cursor: CKQueryOperation.Cursor?

The cursor for continuing the search.

class Cursor

An object that marks the stopping point for a query and the starting point for retrieving the remaining results.

var zoneID: CKRecordZone.ID?

The ID of the record zone that contains the records to search.

var resultsLimit: Int

The maximum number of records to return at one time.

class let maximumResults: Int

A constant value that represents the maximum number of results CloudKit retrieves.

var desiredKeys: [CKRecord.FieldKey]?

The fields of the records to fetch.

### Processing the Query Results

var recordFetchedBlock: ((CKRecord) -> Void)?

The closure to execute when a record becomes available.

Deprecated

var queryCompletionBlock: ((CKQueryOperation.Cursor?, (any Error)?) -> Void)?

The closure to execute after CloudKit retrieves all of the records.

Deprecated

### Instance Properties

var queryResultBlock: ((Result&lt;CKQueryOperation.Cursor?, any Error>) -> Void)?

var recordMatchedBlock: ((CKRecord.ID, Result&lt;CKRecord, any Error>) -> Void)?

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

### Queries

class CKQuery

A query that describes the criteria to apply when searching for records in a database.

class CKLocationSortDescriptor

An object for sorting records that contain location data.

