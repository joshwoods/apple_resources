

- ARKit
- ARSession
-  ARSession.CollaborationData 

Class

# ARSession.CollaborationData

An object that holds information that a user has collected about the physical environment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class CollaborationData
```

## Overview

To create a multiuser AR experience, you enable collaboration on a world tracking session. ARKit regularly outputs ARSession.CollaborationData that users share with each other, which enables everyone to view the same virtual content from their own perspective. For more information, see isCollaborationEnabled.

## Topics

### Observing Priority

var priority: ARSession.CollaborationData.Priority

A property that gives you a hint about how to send a given data instance over the network.

enum Priority

Options that help you choose the appropriate network protocol or settings for a given data instance.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Managing collaboration

func update(with: ARSession.CollaborationData)

Updates your session with information about the physical environment that is collected by another user.

