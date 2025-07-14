

- CloudKit
-  CKSyncEngineZoneDeletionReason 

Enumeration

# CKSyncEngineZoneDeletionReason

Describes the reason for a record zone deletion.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum CKSyncEngineZoneDeletionReason
```

## Topics

### Deletion reasons

case deleted

Your app deleted the record zone.

case encryptedDataReset

The owner of the iCloud account reset their encrypted data.

case purged

The owner of the iCloud account purged your app’s data using the Settings app.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing changes

let deletions: [CKDatabase.DatabaseChange.Deletion]

The fetched record deletions.

let modifications: [CKDatabase.DatabaseChange.Modification]

The fetched record modifications.

