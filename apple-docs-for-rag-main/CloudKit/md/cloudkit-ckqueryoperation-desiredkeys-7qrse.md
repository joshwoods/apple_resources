

- CloudKit
- CKQueryOperation
-  desiredKeys 

Instance Property

# desiredKeys

The fields of the records to fetch.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
var desiredKeys: [CKRecord.FieldKey]? { get set }
```

## Discussion

Use this property to limit the amount of data that CloudKit returns for each record. When CloudKit returns a record, it only includes fields with names that match one of the keys in this property. The property’s default value is `nil`, which instructs CloudKit to return all of a record’s keys.

If you intend to specify a value other than `nil`, do so before you execute the operation or add the operation to a queue.

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

class let maximumResults: Int

A constant value that represents the maximum number of results CloudKit retrieves.

