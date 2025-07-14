

- CloudKit
- CKRecordZone
- CKRecordZone.Capabilities
-  sharing 

Type Property

# sharing

A capability for sharing a specific hierarchy of records.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static var sharing: CKRecordZone.Capabilities { get }
```

## Discussion

CloudKit allows you to share record hierarchies from custom record zones that you create in the user’s private database. For more information, see Shared Records.

## See Also

### Zone Capabilities

static var atomic: CKRecordZone.Capabilities

A capability that allows atomic changes of multiple records.

static var fetchChanges: CKRecordZone.Capabilities

A capability for fetching only the changed records from a zone.

static var zoneWideSharing: CKRecordZone.Capabilities

A capability for sharing the entire contents of a record zone.

