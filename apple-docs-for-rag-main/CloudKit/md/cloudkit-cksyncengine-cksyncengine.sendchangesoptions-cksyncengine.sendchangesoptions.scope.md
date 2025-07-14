

- CloudKit
- CKSyncEngine
- CKSyncEngine.SendChangesOptions
-  CKSyncEngine.SendChangesOptions.Scope 

Enumeration

# CKSyncEngine.SendChangesOptions.Scope

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
enum Scope
```

## Topics

### Enumeration Cases

case all

case allExcluding([CKRecordZone.ID])

case recordIDs([CKRecord.ID])

case zoneIDs([CKRecordZone.ID])

### Instance Methods

func contains(CKRecord.ID) -> Bool

func contains(CKSyncEngine.PendingRecordZoneChange) -> Bool

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Sendable

