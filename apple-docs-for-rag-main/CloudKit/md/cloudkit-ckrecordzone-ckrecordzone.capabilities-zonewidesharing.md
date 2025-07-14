

- CloudKit
- CKRecordZone
- CKRecordZone.Capabilities
-  zoneWideSharing 

Type Property

# zoneWideSharing

A capability for sharing the entire contents of a record zone.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var zoneWideSharing: CKRecordZone.Capabilities { get }
```

## Discussion

CloudKit allows you to share custom record zones that you create in the user’s private database. For more information, see Shared Records.

## See Also

### Zone Capabilities

static var atomic: CKRecordZone.Capabilities

A capability that allows atomic changes of multiple records.

static var fetchChanges: CKRecordZone.Capabilities

A capability for fetching only the changed records from a zone.

static var sharing: CKRecordZone.Capabilities

A capability for sharing a specific hierarchy of records.

