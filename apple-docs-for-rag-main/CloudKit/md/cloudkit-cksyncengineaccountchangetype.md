

- CloudKit
-  CKSyncEngineAccountChangeType 

Enumeration

# CKSyncEngineAccountChangeType

Describes a change to the device’s iCloud account.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum CKSyncEngineAccountChangeType
```

## Topics

### Account change types

case signIn

A change indicating a sign-in to an iCloud account.

case signOut

A change indicating a sign-out of an iCloud account.

case switchAccounts

A change indicating a switch between two iCloud accounts.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

