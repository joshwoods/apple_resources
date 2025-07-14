

- CloudKit
- CKQueryOperation
-  cursor 

Instance Property

# cursor

The cursor for continuing the search.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var cursor: CKQueryOperation.Cursor? { get set }
```

## Discussion

The initial value of this property is the cursor that you provide to the init(cursor:) method. When you use a cursor, the operation ignores the contents of the query property. This property’s value is an opaque value that CloudKit provides. For more information, see the queryCompletionBlock property.

If you intend to specify or change the value in this property, do so before you execute the operation or submit it to a queue.

## See Also

### Configuring the Query Operation

var query: CKQuery?

The query for the search.

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

