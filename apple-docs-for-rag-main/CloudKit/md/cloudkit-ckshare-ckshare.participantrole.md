

- CloudKit
- CKShare
-  CKShare.ParticipantRole 

Enumeration

# CKShare.ParticipantRole

Constants that represent the role of a share’s participant.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum ParticipantRole
```

## Topics

### Roles

case owner

The participant is the share’s owner.

case privateUser

The participant has the private role.

case publicUser

The participant has the public role.

case unknown

The participant’s role is unknown.

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

enum ParticipantPermission

Constants that represent the permissions to grant to a share participant.

var role: CKShare.ParticipantRole

The participant’s role for the share.

typealias Role

A type that represents the role for a participant.

