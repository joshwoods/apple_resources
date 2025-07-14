

- Foundation
- NetService
-  publish(options:) 

Instance Method

# publish(options:)

Attempts to advertise the receiver on the network, with the given options.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.5–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func publish(options: NetService.Options = [])
```

## Parameters 

`options`  

Options for the receiver. The supported options are described in NetService.Options.

## Discussion

This method returns immediately, with success or failure indicated by the callbacks to the delegate.

## See Also

### Using Network Services

func publish()

Attempts to advertise the receiver’s on the network.

Deprecated

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

func stop()

Halts a currently running attempt to publish or resolve a service.

Deprecated

func stopMonitoring()

Stops the monitoring of TXT-record updates for the receiver.

Deprecated

