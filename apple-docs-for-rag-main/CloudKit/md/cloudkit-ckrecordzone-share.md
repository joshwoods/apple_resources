

- CloudKit
- CKRecordZone
-  share 

Instance Property

# share

A reference to the record zone’s share record.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@NSCopying
var share: CKRecord.Reference? { get }
```

## Discussion

CloudKit sets this property only for fetched record zones that contain a share record; otherwise, it’s `nil`.

To share a record zone, create a share record using the init(recordZoneID:) method and then save it to the server. Shared record zones must have the zoneWideSharing capability, which CloudKit enables by default for new custom record zones in the user’s private database.

A record zone, and the records it contains, can take part in only a single share. CloudKit returns an error if you attempt to share an already-shared record zone, or if that record zone contains previously shared records.

Record zone sharing errors include the following:

- CKError.Code.serverRecordChanged, which CloudKit returns if you try to share an already-shared record zone.

- CKError.Code.serverRejectedRequest, which CloudKit returns if you try to share a record hierarchy from an already-shared record zone.

- CKError.Code.invalidArguments, which CloudKit returns if you try to share a record zone that contains one or more shared hierarchies.

