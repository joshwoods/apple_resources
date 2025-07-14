

- Nearby Interaction
- NINearbyObject
-  NINearbyObject.RemovalReason 

Enumeration

# NINearbyObject.RemovalReason

The reason a session removed a nearby object.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
enum RemovalReason
```

## Overview

Each case is a possible value of the `reason` argument to the delegate’s session(_:didRemove:reason:) callback.

## Topics

### Reasons

case peerEnded

The peer ended the session.

case timeout

NI timed out the session.

case peerEnded

The peer ended the session.

case timeout

NI timed out the session.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

