

- CloudKit
- CKRecord
-  CKRecord.FieldKey 

Type Alias

# CKRecord.FieldKey

The data type that CloudKit requires for record field names.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+

``` source
typealias FieldKey = String
```

## See Also

### Creating a Record

convenience init(recordType: CKRecord.RecordType, recordID: CKRecord.ID)

Creates a record using an ID that you provide.

typealias RecordType

The data type that CloudKit requires for record types.

convenience init(recordType: CKRecord.RecordType, zoneID: CKRecordZone.ID)

Creates a record in the specified zone.

Deprecated

