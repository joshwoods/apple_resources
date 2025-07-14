

- Network Extension
- NETunnelProviderSession
-  startTunnel(options:) 

Instance Method

# startTunnel(options:)

Start the process of connecting the tunnel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func startTunnel(options: [String : Any]? = nil) throws
```

## Parameters 

`options`  

A dictionary containing options to be passed to the Tunnel Provider extension.

## Discussion

This method returns immediately after starting the process of connecting the tunnel. In order to be notified when the tunnel is fully connected, register to observe the NEVPNStatusDidChangeNotification notification on the `NETunnelProviderSession` object and examine its status property when the notification is received.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Controlling the tunnel connection

func stopTunnel()

Start the process of disconnecting the tunnel.

