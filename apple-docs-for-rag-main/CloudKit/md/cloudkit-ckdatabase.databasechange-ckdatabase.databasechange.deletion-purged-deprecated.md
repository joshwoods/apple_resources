

- CloudKit
- CKDatabase
- 
  - CKDatabase
- CKDatabase.DatabaseChange
- CKDatabase.DatabaseChange.Deletion
-  purged Deprecated

Instance Property

# purged

A Boolean value that indicates whether the user deleted the record zone when managing their iCloud storage.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 15.0–17.0DeprecatedvisionOSwatchOS 8.0–10.0Deprecated

``` source
var purged: Bool { get }
```

Deprecated

now surfaced as Reason.purged

## See Also

### Identifying the Deleted Record Zone

var zoneID: CKRecordZone.ID

The identifier of the deleted record zone.

