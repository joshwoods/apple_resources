

- Foundation
- NetService
-  resolve() Deprecated

Instance Method

# resolve()

Starts a resolve process for the service.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func resolve()
```

Deprecated

Use resolve(withTimeout:) instead.

## Discussion

Attempts to determine at least one address for the service. This method returns immediately, with success or failure indicated by the callbacks to the delegate.

In OS X v10.4, this method calls resolve(withTimeout:) with a timeout value of `5`.

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

func resolve(withTimeout: TimeInterval)

Starts a resolve process of a finite duration for the service.

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

