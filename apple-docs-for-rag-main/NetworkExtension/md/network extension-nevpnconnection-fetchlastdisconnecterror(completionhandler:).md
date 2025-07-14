

- Network Extension
- NEVPNConnection
-  fetchLastDisconnectError(completionHandler:) 

Instance Method

# fetchLastDisconnectError(completionHandler:)

Retrives the most recent error that caused the VPN to disconnect.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+visionOS 1.0+

``` source
func fetchLastDisconnectError(completionHandler handler: @escaping ((any Error)?) -> Void)
```

``` source
func fetchLastDisconnectError() async throws
```

## Parameters 

`handler`  

An error handler that receives the last disconnect error as a parameter.

## Discussion

If VPN system (including the IPsec client) generated the error, then the error uses the NEVPNConnectionErrorDomain error domain. If the error came from a tunnel provider app extension instead, then the error is the NSError that the provider passed when disconnecting the tunnel.

## See Also

### Handling errors

let NEVPNConnectionErrorDomain: String

The domain for errors resulting from VPN connection calls.

enum NEVPNConnectionError

Error codes specific to VPN connections.

