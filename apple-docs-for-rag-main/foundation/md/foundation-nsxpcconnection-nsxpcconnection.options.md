

- Foundation
- NSXPCConnection
-  NSXPCConnection.Options 

Structure

# NSXPCConnection.Options

Options that you can pass to a connection.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Options
```

## Topics

### Constants

static var privileged: NSXPCConnection.Options

static var privileged: NSXPCConnection.Options

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Creating a connection

init(listenerEndpoint: NSXPCListenerEndpoint)

Initializes an NSXPCConnection object to connect to an NSXPCListener object in another process, identified by an NSXPCListenerEndpoint object.

init(machServiceName: String, options: NSXPCConnection.Options)

Initializes an NSXPCConnection object to connect to a LaunchAgent or LaunchDaemon with a name advertised in a `launchd.plist`.

init(serviceName: String)

Initializes an NSXPCConnection object to connect to an NSXPCListener object in an XPC service, identified by a service name.

