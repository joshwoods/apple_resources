

- Network Extension
- NETunnelProviderSession
-  stopTunnel() 

Instance Method

# stopTunnel()

Start the process of disconnecting the tunnel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func stopTunnel()
```

## Discussion

This method returns immediately after starting the process of disconnecting the tunnel. In order to be notified when the tunnel is fully disconnected, register to observe the NEVPNStatusDidChangeNotification notification on the NETunnelProviderSession object and examine its status property when the notification is received.

## See Also

### Controlling the tunnel connection

func startTunnel(options: [String : Any]?) throws

Start the process of connecting the tunnel.

