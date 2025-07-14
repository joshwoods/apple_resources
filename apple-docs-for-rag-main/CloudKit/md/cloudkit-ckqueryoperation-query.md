

- CloudKit
- CKQueryOperation
-  query 

Instance Property

# query

The query for the search.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var query: CKQuery? { get set }
```

## Discussion

The initial value of this property is the query that you provide to the init(query:) method. When the value in the cursor property is `nil`, the operation uses this property’s value to execute a new search and return its results to your completion handler. If cursor isn’t `nil`, the operation uses the cursor instead.

If you intend to specify or change the value of this property, do so before you execute the operation or submit it to a queue.

## See Also

### Configuring the Query Operation

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

