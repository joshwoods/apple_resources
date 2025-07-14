

- CloudKit
- CKSyncEngine
-  CKSyncEngine.SendChangesContext 

Structure

# CKSyncEngine.SendChangesContext

A type that describes a single attempt to send changes to the iCloud servers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct SendChangesContext
```

## Overview

A sync engine has two ways to send changes to iCloud — periodically, in cooperation with the system scheduler, and manually, whenever your app invokes the sendChanges(_:) method. This type provides information about a single attempt to send changes that includes both the reason for the attempt and any additional options in use by the attempt.

## Topics

### Accessing specific attributes

let reason: CKSyncEngine.SyncReason

The reason for the send operation.

enum SyncReason

Describes the reason for a sync operation.

enum CKSyncEngineSyncReason

Describes the reason for a sync operation.

let options: CKSyncEngine.SendChangesOptions

The additional options for the send operation.

struct SendChangesOptions

A set of options to use with a send operation.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Sending changes

func nextRecordZoneChangeBatch(CKSyncEngine.SendChangesContext, syncEngine: CKSyncEngine) async -> CKSyncEngine.RecordZoneChangeBatch?

Asks the delegate to provide the next set of record changes to send to the server.

**Required**

struct RecordZoneChangeBatch

A type that contains the record changes for a single send operation.

