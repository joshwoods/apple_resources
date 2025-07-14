

- CloudKit
- CKShare
- CKShare.Metadata
-  rootRecordID Deprecated

Instance Property

# rootRecordID

The record ID of the share’s root record.

iOS 10.0–16.0DeprecatediPadOS 10.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.12–13.0DeprecatedtvOS 10.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–9.0Deprecated

``` source
@NSCopying
var rootRecordID: CKRecord.ID { get }
```

Deprecated

Use hierarchicalRootRecordID instead.

## Discussion

CloudKit populates this property only for metadata that belongs to a shared record hierarchy. If the metadata is part of a shared record zone, the property returns `nil`. This is because, unlike a shared record hierarchy, a shared record zone doesn’t have a nominated root record.

## See Also

### Accessing the Root Record

var hierarchicalRootRecordID: CKRecord.ID?

The record ID of the shared hierarchy’s root record.

var rootRecord: CKRecord?

The share’s root record.

