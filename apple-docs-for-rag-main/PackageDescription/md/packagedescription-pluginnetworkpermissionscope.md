

- PackageDescription
-  PluginNetworkPermissionScope 

Enumeration

# PluginNetworkPermissionScope

The scope of a network permission.

SwiftPM 5.9+

``` source
enum PluginNetworkPermissionScope
```

## Overview

The scope can be none, local connections only, or all connections.

## Topics

### Enumeration Cases

case all(ports: [Int])

Allow local and outgoing network connections; can be limited to a list of allowed ports.

case docker

Allow connections to Docker through UNIX domain sockets.

case local(ports: [Int])

Allow local network connections; can be limited to a list of allowed ports.

case none

Do not allow network access.

case unixDomainSocket

Allow connections to any UNIX domain socket.

### Type Methods

static func all(ports: Range&lt;Int>) -> PluginNetworkPermissionScope

Allow local and outgoing network connections, limited to a range of allowed ports.

static func local(ports: Range&lt;Int>) -> PluginNetworkPermissionScope

Allow local network connections, limited to a range of allowed ports.

