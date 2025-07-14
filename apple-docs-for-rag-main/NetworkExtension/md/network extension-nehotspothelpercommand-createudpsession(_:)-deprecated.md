

- Network Extension
- NEHotspotHelperCommand
-  createUDPSession(\_:) Deprecated

Instance Method

# createUDPSession(\_:)

Creates a new UDP session over the network associated with the command.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func createUDPSession(_ endpoint: NWEndpoint) -> NWUDPSession
```

Deprecated

Pass the Swift interface property or the ObjectiveC interface property to the nw_parameters_require_interface(_:_:) function from the Network framework instead.

## Parameters 

`endpoint`  

The remote host and port of the session.

## Return Value

A UDP session that will connect over the network associated with the command.

## Discussion

The UDP session is started automatically. Use KVO to observe the session’s state property to be notified when the session is ready to send and receive UDP datagrams. For information about KVO see Key-Value Observing Programming Guide.

## See Also

### Networking on the hotspot network

func bind(to: NEHotspotHelperCommand)

Binds a URL request to the network interface associated with the hotspot helper command instance.

func createTCPConnection(NWEndpoint) -> NWTCPConnection

Create a new TCP connection over the network associated with the command.

Deprecated

