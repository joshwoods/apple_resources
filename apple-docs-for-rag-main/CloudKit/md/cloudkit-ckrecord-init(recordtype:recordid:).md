

- CloudKit
- CKRecord
-  init(recordType:recordID:) 

Initializer

# init(recordType:recordID:)

Creates a record using an ID that you provide.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
convenience init(
    recordType: CKRecord.RecordType,
    recordID: CKRecord.ID = CKRecord.ID()
)
```

## Parameters 

`recordType`  

A string that represents the type of record that you want to create. You can’t change the record type after initialization. You define the record types that your app supports and use them to distinguish between records with different types of data. This parameter must not be `nil` or contain an empty string.

A record type must consist of one or more alphanumeric characters and must start with a letter. CloudKit permits the use of underscores, but not spaces.

`recordID`  

The ID to assign to the record. When creating the ID, you can specify the zone where you want to store the record. The ID must be unique across all records and can’t be `nil`.

## Discussion

Use this method to initialize a new record object with the specified ID. The newly created record contains no data.

Upon creation, record objects exist only in memory on the local device. Save the record using a CKModifyRecordsOperation object or by using the save(_:completionHandler:) method to transfer the record’s contents to the server.

## See Also

### Creating a Record

typealias RecordType

The data type that CloudKit requires for record types.

typealias FieldKey

The data type that CloudKit requires for record field names.

convenience init(recordType: CKRecord.RecordType, zoneID: CKRecordZone.ID)

Creates a record in the specified zone.

Deprecated

