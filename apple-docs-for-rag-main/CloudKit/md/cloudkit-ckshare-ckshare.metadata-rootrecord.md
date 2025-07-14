

- CloudKit
- CKShare
- CKShare.Metadata
-  rootRecord 

Instance Property

# rootRecord

The share’s root record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var rootRecord: CKRecord? { get }
```

## Discussion

This property contains the root record of the shared record hierarchy if you set the shouldFetchRootRecord property of the operation that fetches the metadata to true. You can specify which fields CloudKit returns by setting the same operation’s rootRecordDesiredKeys property.

The operation ignores the shouldFetchRootRecord and rootRecordDesiredKeys properties when fetching a shared record zone’s metadata because, unlike a shared record hierarchy, a record zone doesn’t have a nominated root record.

## See Also

### Accessing the Root Record

var hierarchicalRootRecordID: CKRecord.ID?

The record ID of the shared hierarchy’s root record.

var rootRecordID: CKRecord.ID

The record ID of the share’s root record.

Deprecated

