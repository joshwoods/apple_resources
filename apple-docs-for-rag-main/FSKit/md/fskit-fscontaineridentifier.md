

- FSKit
-  FSContainerIdentifier 

Class

# FSContainerIdentifier

A type that identifies a container.

macOS 15.4+

``` source
class FSContainerIdentifier
```

## Overview

The identifier is either a UUID or a UUID with additional differentiating bytes. Some network protocols evaluate access based on a user ID when connecting. In this situation, when a file server receives multiple client connections with different user IDs, the server provides different file hierarchies to each. For such systems, represent the container identifier as the UUID associated with the server, followed by four or eight bytes to differentiate connections.

Important

Don’t subclass this class.

## Topics

### Accessing identifier properties

var volumeIdentifier: FSVolume.Identifier

The volume identifier associated with the container.

## Relationships

### Inherits From

- FSEntityIdentifier

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Identifiable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Containers

class FSContainerStatus

A type that represents a container’s status.

