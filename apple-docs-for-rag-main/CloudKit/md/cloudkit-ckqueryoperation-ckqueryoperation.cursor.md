

- CloudKit
- CKQueryOperation
-  CKQueryOperation.Cursor 

Class

# CKQueryOperation.Cursor

An object that marks the stopping point for a query and the starting point for retrieving the remaining results.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class Cursor
```

## Overview

You don’t create instances of this class yourself. When fetching records using a query operation, if the number of results exceeds the limit for the query, CloudKit provides a cursor. Use that cursor to create a new instance of CKQueryOperation and retrieve the next batch of results for the same query.

For information about how to use a CKQueryOperation.Cursor object, see CKQueryOperation.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Configuring the Query Operation

var query: CKQuery?

The query for the search.

var cursor: CKQueryOperation.Cursor?

The cursor for continuing the search.

var zoneID: CKRecordZone.ID?

The ID of the record zone that contains the records to search.

var resultsLimit: Int

The maximum number of records to return at one time.

class let maximumResults: Int

A constant value that represents the maximum number of results CloudKit retrieves.

var desiredKeys: [CKRecord.FieldKey]?

The fields of the records to fetch.

