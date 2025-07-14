

- Foundation
- NetService
-  resolve(withTimeout:) Deprecated

Instance Method

# resolve(withTimeout:)

Starts a resolve process of a finite duration for the service.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func resolve(withTimeout timeout: TimeInterval)
```

Deprecated

Use nw_connection_t or nw_listener_t in Network framework instead

## Parameters 

`timeout`  

The maximum number of seconds to attempt a resolve. A value of 0.0 indicates no timeout and a resolve process of indefinite duration.

## Discussion

During the resolve period, the service sends netServiceDidResolveAddress(_:) to the delegate for each address it discovers that matches the service parameters. Once the timeout is hit, the service sends netServiceDidStop(_:) to the delegate. If no addresses resolve during the timeout period, the service sends netService(_:didNotResolve:) to the delegate.

## See Also

### Related Documentation

var addresses: [Data]?

A read-only array containing `NSData` objects, each of which contains a socket address for the service.

Deprecated

### Using Network Services

func publish()

Attempts to advertise the receiver’s on the network.

Deprecated

func publish(options: NetService.Options)

Attempts to advertise the receiver on the network, with the given options.

func resolve()

Starts a resolve process for the service.

Deprecated

var port: Int

The port on which the service is listening for connections.

func startMonitoring()

Starts the monitoring of TXT-record updates for the receiver.

Deprecated

func stop()

Halts a currently running attempt to publish or resolve a service.

Deprecated

func stopMonitoring()

Stops the monitoring of TXT-record updates for the receiver.

Deprecated

