

- PushKit
-  PKPushType 

Structure

# PKPushType

Constants reflecting the push types you want to support.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
struct PKPushType
```

## Topics

### Notification Types

static let complication: PKPushType

A push type for watchOS complications.

Deprecated

static let fileProvider: PKPushType

A push type for file provider updates.

static let voIP: PKPushType

A push type for Voice-over-IP (VoIP) call invitations.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Push Types

Responding to VoIP Notifications from PushKit

Receive incoming Voice-over-IP (VoIP) push notifications and use them to display the system call interface to the user.

