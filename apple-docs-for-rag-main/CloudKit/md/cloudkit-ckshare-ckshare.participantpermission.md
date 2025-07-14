

- CloudKit
- CKShare
-  CKShare.ParticipantPermission 

Enumeration

# CKShare.ParticipantPermission

Constants that represent the permissions to grant to a share participant.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum ParticipantPermission
```

## Topics

### Permissions

case none

The participant doesn’t have any permissions for the share.

case readOnly

The participant has read-only permissions for the share.

case readWrite

The participant has read-and-write permissions for the share.

case unknown

The participant’s permissions are unknown.

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

### Managing the Participant’s Capabilites

var permission: CKShare.ParticipantPermission

The participant’s permission level for the share.

typealias Permission

A type that represents the permissions for a participant.

var role: CKShare.ParticipantRole

The participant’s role for the share.

typealias Role

A type that represents the role for a participant.

enum ParticipantRole

Constants that represent the role of a share’s participant.

