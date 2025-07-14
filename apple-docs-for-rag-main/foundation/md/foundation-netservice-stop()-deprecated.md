

- Foundation
- NetService
-  stop() Deprecated

Instance Method

# stop()

Halts a currently running attempt to publish or resolve a service.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func stop()
```

Deprecated

Use nw_connection_t or nw_listener_t in Network framework instead

## Discussion

The delegate will receive netServiceDidStop(_:) after the service stops.

It is safe to remove all strong references to the service immediately after calling stop().

## See Also

### Using Network Services

func publish()

Attempts to advertise the receiver’s on the network.

Deprecated

func publish(options: NetService.Options)

Attempts to advertise the receiver on the network, with the given options.

func resolve()

Starts a resolve process for the service.

Deprecated

func resolve(withTimeout: TimeInterval)

Starts a resolve process of a finite duration for the service.

Deprecated

var port: Int

The port on which the service is listening for connections.

func startMonitoring()

Starts the monitoring of TXT-record updates for the receiver.

Deprecated

func stopMonitoring()

Stops the monitoring of TXT-record updates for the receiver.

Deprecated

