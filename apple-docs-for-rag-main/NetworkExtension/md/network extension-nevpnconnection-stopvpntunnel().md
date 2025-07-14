

- Network Extension
- NEVPNConnection
-  stopVPNTunnel() 

Instance Method

# stopVPNTunnel()

Start the process of disconnecting the VPN.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func stopVPNTunnel()
```

## Discussion

This method returns immediately after starting the process of disconnecting the VPN. In order to be notified when the VPN is fully disconnected, register to observe the NEVPNStatusDidChangeNotification notification on the NEVPNConnection object and examine the status property when the notification is received.

## See Also

### Controlling the VPN connection

func startVPNTunnel() throws

Start the process of connecting the VPN.

func startVPNTunnel(options: [String : NSObject]?) throws

Start the process of connecting the VPN.

let NEVPNConnectionStartOptionUsername: String

let NEVPNConnectionStartOptionPassword: String

