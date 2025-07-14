

- Network Extension
- NEPacketTunnelProvider
-  stopTunnel(with:completionHandler:) 

Instance Method

# stopTunnel(with:completionHandler:)

Stop the network tunnel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func stopTunnel(
    with reason: NEProviderStopReason,
    completionHandler: @escaping () -> Void
)
```

``` source
func stopTunnel(with reason: NEProviderStopReason) async
```

## Parameters 

`reason`  

An `NEProviderStopReason` code indicating why the tunnel is being stopped. Possible codes are listed in NEProvider.

`completionHandler`  

A block that must be executed when the tunnel is fully stopped.

## Discussion

This method is called by the system to stop the network tunnel.

NEPacketTunnelProvider subclasses must override this method.

Do not use this method to stop the tunnel from the Packet Tunnel Provider. Use `cancelTunnelWithError`: instead.

## See Also

### Managing the tunnel life cycle

func startTunnel(options: [String : NSObject]?, completionHandler: ((any Error)?) -> Void)

Start the network tunnel.

func cancelTunnelWithError((any Error)?)

Stop the network tunnel from the Packet Tunnel Provider.

