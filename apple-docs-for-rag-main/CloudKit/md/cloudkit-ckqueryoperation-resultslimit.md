

- CloudKit
- CKQueryOperation
-  resultsLimit 

Instance Property

# resultsLimit

The maximum number of records to return at one time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var resultsLimit: Int { get set }
```

## Discussion

For most queries, leave the value of this property as the default value, which is the maximumResults constant. When using that value, CloudKit returns as many records as possible while minimizing delays in receiving those records. If you want to process a fixed number of results, change the value of this property accordingly.

## See Also

### Configuring the Query Operation

var query: CKQuery?

The query for the search.

var cursor: CKQueryOperation.Cursor?

The cursor for continuing the search.

class Cursor

An object that marks the stopping point for a query and the starting point for retrieving the remaining results.

var zoneID: CKRecordZone.ID?

The ID of the record zone that contains the records to search.

class let maximumResults: Int

A constant value that represents the maximum number of results CloudKit retrieves.

var desiredKeys: [CKRecord.FieldKey]?

The fields of the records to fetch.

