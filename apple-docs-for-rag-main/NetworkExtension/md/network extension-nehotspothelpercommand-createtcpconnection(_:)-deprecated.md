

- Network Extension
- NEHotspotHelperCommand
-  createTCPConnection(\_:) Deprecated

Instance Method

# createTCPConnection(\_:)

Create a new TCP connection over the network associated with the command.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func createTCPConnection(_ endpoint: NWEndpoint) -> NWTCPConnection
```

Deprecated

Pass the Swift interface property or the ObjectiveC interface property to the nw_parameters_require_interface(_:_:) function from the Network framework instead.

## Parameters 

`endpoint`  

The remote host and port of the connection.

## Return Value

A TCP connection that will connect over the network associated with the command.

## Discussion

The TCP connection is started automatically. Use KVO to observe the connection’s `state` property to be notified when the connection is established or fails.

## See Also

### Networking on the hotspot network

func bind(to: NEHotspotHelperCommand)

Binds a URL request to the network interface associated with the hotspot helper command instance.

func createUDPSession(NWEndpoint) -> NWUDPSession

Creates a new UDP session over the network associated with the command.

Deprecated

