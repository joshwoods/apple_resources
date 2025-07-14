

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.AccountChange 

Structure

# CKSyncEngine.Event.AccountChange

A type that provides information about a change to the device’s iCloud account.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct AccountChange
```

## Overview

Important

When a sync engine detects a change to the device’s iCloud account, it resets its internal state, including unsaved changes to both records and record zones. Your app needs to handle this scenario gracefully.

## Topics

### Understanding the change

let changeType: CKSyncEngine.Event.AccountChange.ChangeType

The iCloud account’s change type.

enum ChangeType

Describes a change to the device’s iCloud account.

enum CKSyncEngineAccountChangeType

Describes a change to the device’s iCloud account.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Account changes

case accountChange(CKSyncEngine.Event.AccountChange)

An event indicating a change to the device’s iCloud account.

