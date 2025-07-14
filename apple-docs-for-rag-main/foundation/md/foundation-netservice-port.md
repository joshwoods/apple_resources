

- Foundation
- NetService
-  port 

Instance Property

# port

The port on which the service is listening for connections.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.5–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
var port: Int { get }
```

## Discussion

If the object was initialized by calling init(domain:type:name:port:) (whether by your code or by a browser object), then the value was set when the object was first initialized.

If the object was initialized by calling init(domain:type:name:), the value of this property is not valid (`-1`) until after the service has successfully been resolved (when `addresses` is non-`nil`).

Backward Compatibility Note

This became a property in OS X v10.9 and iOS 7, but the underlying getter method (`port`) has been available since this class was first introduced.

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

func startMonitoring()

Starts the monitoring of TXT-record updates for the receiver.

Deprecated

func stop()

Halts a currently running attempt to publish or resolve a service.

Deprecated

func stopMonitoring()

Stops the monitoring of TXT-record updates for the receiver.

Deprecated

