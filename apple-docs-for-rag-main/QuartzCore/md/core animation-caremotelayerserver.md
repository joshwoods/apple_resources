

- Core Animation
-  CARemoteLayerServer 

Class

# CARemoteLayerServer

A legacy class for cross-process rendering.

Mac Catalyst 13.1+macOS 10.7+

``` source
class CARemoteLayerServer
```

## Overview

`CARemoteLaterServer` is a legacy class for cross-process rendering. IOSurfaceCreateMachPort(_:) and IOSurfaceCreateXPCObject(_:), available with IOSurface, offer an improved way to perform cross-process rendering.

## Topics

### Creating a Server

var serverPort: mach_port_t

The port number of the server.

### Getting a Server Instance

class func shared() -> CARemoteLayerServer

Returns the (singleton) instance of the shared remote layer server.

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

class CARemoteLayerClient

A legacy class for cross-process rendering.

