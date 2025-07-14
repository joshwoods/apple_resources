

- CloudKit
- CKQueryOperation
-  zoneID 

Instance Property

# zoneID

The ID of the record zone that contains the records to search.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var zoneID: CKRecordZone.ID? { get set }
```

## Discussion

The value of this property limits the scope of the search to only the records in the specified record zone. If you don’t specify a record zone, the search includes all record zones.

When you create an operation using the init(cursor:) method, this property’s value is `nil` and CloudKit ignores any changes that you make to it. When the operation executes, the cursor provides the record zone information from the original search that provides the cursor.

## See Also

### Configuring the Query Operation

var query: CKQuery?

The query for the search.

var cursor: CKQueryOperation.Cursor?

The cursor for continuing the search.

class Cursor

An object that marks the stopping point for a query and the starting point for retrieving the remaining results.

var resultsLimit: Int

The maximum number of records to return at one time.

class let maximumResults: Int

A constant value that represents the maximum number of results CloudKit retrieves.

var desiredKeys: [CKRecord.FieldKey]?

The fields of the records to fetch.

