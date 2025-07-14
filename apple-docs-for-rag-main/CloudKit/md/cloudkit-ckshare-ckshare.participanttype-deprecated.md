

- CloudKit
- CKShare
-  CKShare.ParticipantType Deprecated

Enumeration

# CKShare.ParticipantType

The role of a participant.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–5.0Deprecated

``` source
enum ParticipantType
```

## Topics

### Constants

case owner

The participant is the share’s owner.

case privateUser

The participant has the private role.

case publicUser

The participant has the public role.

case unknown

The participant’s role is unknown.

case unknown

An unknown role.

case owner

The type of an owner.

case privateUser

The type of a private user.

case publicUser

The type of a public owner.

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

### Deprecated Properties

var type: CKShare.ParticipantType

The participant type.

Deprecated

typealias ParticipantType

A type that represents the role of the participant.

