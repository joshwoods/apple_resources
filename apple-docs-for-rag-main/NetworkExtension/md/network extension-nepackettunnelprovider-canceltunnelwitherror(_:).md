

- Network Extension
- NEPacketTunnelProvider
-  cancelTunnelWithError(\_:) 

Instance Method

# cancelTunnelWithError(\_:)

Stop the network tunnel from the Packet Tunnel Provider.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func cancelTunnelWithError(_ error: (any Error)?)
```

## Parameters 

`error`  

An NSError object containing the error that caused the tunnel to be stopped. The domain and code of this NSError object is defined by the caller.

## Discussion

The Packet Tunnel Provider should call this method when an unrecoverable error occurs, such as the tunnel server going down or the VPN authentication session expiring.

## See Also

### Managing the tunnel life cycle

func startTunnel(options: [String : NSObject]?, completionHandler: ((any Error)?) -> Void)

Start the network tunnel.

func stopTunnel(with: NEProviderStopReason, completionHandler: () -> Void)

Stop the network tunnel.

