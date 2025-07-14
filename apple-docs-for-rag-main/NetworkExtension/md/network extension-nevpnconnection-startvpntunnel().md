

- Network Extension
- NEVPNConnection
-  startVPNTunnel() 

Instance Method

# startVPNTunnel()

Start the process of connecting the VPN.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func startVPNTunnel() throws
```

## Discussion

This method returns immediately after starting the process of connecting the VPN. In order to be notified when the VPN is fully connected, register to observe the NEVPNStatusDidChangeNotification notification on the NEVPNConnection object, and examine the status property when the notification is received.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Controlling the VPN connection

func startVPNTunnel(options: [String : NSObject]?) throws

Start the process of connecting the VPN.

let NEVPNConnectionStartOptionUsername: String

let NEVPNConnectionStartOptionPassword: String

func stopVPNTunnel()

Start the process of disconnecting the VPN.

