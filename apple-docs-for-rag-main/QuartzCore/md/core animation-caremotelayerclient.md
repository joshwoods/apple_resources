

- Core Animation
-  CARemoteLayerClient 

Class

# CARemoteLayerClient

A legacy class for cross-process rendering.

Mac Catalyst 13.1+macOS 10.7+

``` source
class CARemoteLayerClient
```

## Overview

`CARemoteLaterClient` is a legacy class for cross-process rendering. IOSurfaceCreateMachPort(_:) and IOSurfaceCreateXPCObject(_:), available with IOSurface, offer an improved way to perform cross-process rendering.

## Topics

### Creating a Client

init(serverPort: mach_port_t)

Creates a layer client from a server port.

### Retrieving Client Properties

var clientId: UInt32

The ID of the remote layer client.

var layer: CALayer?

The layer associated with the remote client.

### Invalidating a Client

func invalidate()

Invalidates a remote layer client.

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

## See Also

### Remote Display of Layer Content

class CARemoteLayerServer

A legacy class for cross-process rendering.

