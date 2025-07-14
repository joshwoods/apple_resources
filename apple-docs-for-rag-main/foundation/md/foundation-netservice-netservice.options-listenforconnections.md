

- Foundation
- NetService
- NetService.Options
-  listenForConnections 

Type Property

# listenForConnections

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
static var listenForConnections: NetService.Options { get }
```

## Discussion

Specifies that a TCP listener should be started for both IPv4 and IPv6 on the port specified by this service. If the listening port can’t be opened, the service calls its delegate’s netService(_:didNotPublish:) method to report the error.

The listener supports only TCP connections. If the service’s type does not end with `_tcp`, publication fails with NetService.ErrorCode.badArgumentError.

Whenever a client connects to the listening socket, the service calls its delegate’s netService(_:didAcceptConnectionWith:outputStream:) method with a pair of `NSStream` objects.

## See Also

### Constants

static var noAutoRename: NetService.Options

Specifies that the network service should not rename itself in the event of a name collision.

static var noAutoRename: NetService.Options

Specifies that the network service should not rename itself in the event of a name collision.

