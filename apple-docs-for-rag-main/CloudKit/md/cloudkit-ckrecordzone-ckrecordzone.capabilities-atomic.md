

- CloudKit
- CKRecordZone
- CKRecordZone.Capabilities
-  atomic 

Type Property

# atomic

A capability that allows atomic changes of multiple records.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
static var atomic: CKRecordZone.Capabilities { get }
```

## Discussion

When you use a CKModifyRecordsOperation object to save records, if the server is unable to save the changes for one record, it doesn’t save the changes for any of the records. Combining this capability with the CKModifyRecordsOperation.RecordSavePolicy.ifServerRecordUnchanged policy of the operation object prevents your app from overwriting changes to a group of records if one or more of the records on the server has recent changes.

## See Also

### Zone Capabilities

static var fetchChanges: CKRecordZone.Capabilities

A capability for fetching only the changed records from a zone.

static var sharing: CKRecordZone.Capabilities

A capability for sharing a specific hierarchy of records.

static var zoneWideSharing: CKRecordZone.Capabilities

A capability for sharing the entire contents of a record zone.

