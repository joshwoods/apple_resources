

- Network Extension
-  NEVPNConnectionErrorDomain 

Global Variable

# NEVPNConnectionErrorDomain

The domain for errors resulting from VPN connection calls.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+visionOS 1.0+

``` source
let NEVPNConnectionErrorDomain: String
```

## Discussion

Match this constant to the domain of an NSError encountered when calling methods on NEVPNConnection. The NEDNSSettingsManagerError enumeration defines possible code values for these errors.

## See Also

### Handling errors

func fetchLastDisconnectError(completionHandler: ((any Error)?) -> Void)

Retrives the most recent error that caused the VPN to disconnect.

enum NEVPNConnectionError

Error codes specific to VPN connections.

