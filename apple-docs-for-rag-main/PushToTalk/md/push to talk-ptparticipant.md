

- Push to Talk
-  PTParticipant 

Class

# PTParticipant

An object that represents a participant.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
class PTParticipant
```

## Overview

Use a PTParticipant object with setActiveRemoteParticipant(_:channelUUID:completionHandler:) to update the name and `imageFileURL` the system displays in the user interface.

## Topics

### Creating a participant

init(name: String, image: UIImage?)

Creates a participant with the name and image you specify.

### Inspecting a participant

var name: String

The name of the participant.

var image: UIImage?

The image file you associate with the participant.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

