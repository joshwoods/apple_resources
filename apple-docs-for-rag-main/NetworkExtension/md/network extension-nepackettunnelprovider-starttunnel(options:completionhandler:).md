

- Network Extension
- NEPacketTunnelProvider
-  startTunnel(options:completionHandler:) 

Instance Method

# startTunnel(options:completionHandler:)

Start the network tunnel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func startTunnel(
    options: [String : NSObject]? = nil,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func startTunnel(options: [String : NSObject]? = nil) async throws
```

## Parameters 

`options`  

A dictionary passed by the app that requested that the tunnel be started. If the starting app did not specify a dictionary of options then this parameter will be nil. If the tunnel was started via Connect On Demand, then this parameter will be nil.

`completionHandler`  

A block that must be executed when the tunnel is fully established, or when the tunnel cannot be started due to an error. If the tunnel was successfully established, then the error parameter must be set to nil. If an error occurred, the error parameter passed to this block must be set to a non-nil NSError object.

## Discussion

This method is called by the system to start the network tunnel.

`NEPacketTunnelProvider` subclasses must override this method.

When the Packet Tunnel Provider executes the completionHandler block with a nil error parameter, it signals to the system that it is ready to begin handling network data. Therefore, the Packet Tunnel Provider should call setTunnelNetworkSettings(_:completionHandler:) and wait for it to complete before executing the completionHandler block.

The domain and code of the NSError object passed to the `completionHandler` block are defined by the Packet Tunnel Provider.

## See Also

### Managing the tunnel life cycle

func stopTunnel(with: NEProviderStopReason, completionHandler: () -> Void)

Stop the network tunnel.

func cancelTunnelWithError((any Error)?)

Stop the network tunnel from the Packet Tunnel Provider.

