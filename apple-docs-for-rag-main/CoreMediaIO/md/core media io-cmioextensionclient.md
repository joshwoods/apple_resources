

- Core Media I/O
-  CMIOExtensionClient 

Class

# CMIOExtensionClient

An object that represents a client of the extension.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionClient
```

## Topics

### Identifying a Client

var clientID: UUID

A unique client identifier.

var pid: pid_t

The process identifier of the client.

### Instance Properties

var signingID: String?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Streams

class CMIOExtensionStream

An object that represents a stream of media data.

protocol CMIOExtensionStreamSource

A protocol for objects that act as stream sources.

class CMIOExtensionStreamProperties

An object that describes the properties of an extension stream.

