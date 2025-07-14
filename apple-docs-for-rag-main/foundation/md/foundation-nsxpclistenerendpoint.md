

- Foundation
-  NSXPCListenerEndpoint 

Class

# NSXPCListenerEndpoint

An object that names a specific XPC listener.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSXPCListenerEndpoint
```

## Overview

An instance of NSXPCListenerEndpoint may be retrieved from an NSXPCListener instance and sent over existing NSXPCConnections. A process may then use the endpoint to create a new NSXPCConnection to the original NSXPCListener.

This pattern is useful if you have a service which multiplexes work to other services. The service can act as an intermediate helper. The requesting application does not need to know specifically which service it is connecting to, just that it implements a known NSXPCInterface.

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

### XPC Services

class NSXPCListener

A listener that waits for new incoming connections, configures them, and accepts or rejects them.

protocol NSXPCListenerDelegate

The protocol that delegates to the XPC listener use to accept or reject new connections.

