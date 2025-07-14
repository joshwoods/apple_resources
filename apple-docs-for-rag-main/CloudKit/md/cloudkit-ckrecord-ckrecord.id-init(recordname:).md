

- CloudKit
- CKRecord
- CKRecord.ID
-  init(recordName:) 

Initializer

# init(recordName:)

Creates a new record ID with the specified name in the default zone.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
convenience init(recordName: String)
```

## Parameters 

`recordName`  

The name that identifies the record. The string must contain only ASCII characters, must not exceed 255 characters, and must not start with an underscore. If you specify `nil` or an empty string for this parameter, the method throws an exception.

## Return Value

An initialized record ID object, or `nil` if CloudKit can’t create the object.

## Discussion

Use this method when you’re creating or searching for records in the default zone.

## See Also

### Creating a Record ID

convenience init(recordName: String, zoneID: CKRecordZone.ID)

Creates a new record ID with the specified name and zone information.

let CKRecordNameZoneWideShare: String

The name of a share record that manages a shared record zone.

