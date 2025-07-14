

- CloudKit
- CKQueryOperation
-  maximumResults 

Type Property

# maximumResults

A constant value that represents the maximum number of results CloudKit retrieves.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class let maximumResults: Int
```

## Discussion

The value of this constant doesn’t correspond to the actual number of records. CloudKit dynamically determines the actual number according to various conditions at runtime.

This constant is the resultsLimit property’s default value.

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

var resultsLimit: Int

The maximum number of records to return at one time.

var desiredKeys: [CKRecord.FieldKey]?

The fields of the records to fetch.

