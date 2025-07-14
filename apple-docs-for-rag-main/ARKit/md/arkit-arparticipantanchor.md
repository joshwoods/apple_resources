

- ARKit
-  ARParticipantAnchor 

Class

# ARParticipantAnchor

An anchor for another user in multiuser augmented reality experiences.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARParticipantAnchor
```

## Overview

When you set isCollaborationEnabled to true, ARKit calls session(_:didAdd:) with an ARParticipantAnchor for every user it detects in your physical environment, providing you with their world position.

## Relationships

### Inherits From

- ARAnchor

### Conforms To

- ARAnchorCopying
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Shared Experiences

Streaming an AR experience

Control an AR experience remotely by transferring sensor and user input over the network.

Creating a collaborative session

Enable nearby devices to share an AR experience by using a peer-to-peer multiuser strategy.

Creating a multiuser AR experience

Enable nearby devices to share an AR experience by using a host-guest multiuser strategy.

class CollaborationData

An object that holds information that a user has collected about the physical environment.

