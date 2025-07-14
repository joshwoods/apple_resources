

- Network Extension
-  NEVPNConnectionError 

Enumeration

# NEVPNConnectionError

Error codes specific to VPN connections.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+visionOS 1.0+

``` source
enum NEVPNConnectionError
```

## Topics

### General error codes

case overslept

An error code that indicates the system slept for an extended period of time, causing the VPN connection to terminate.

case noNetworkAvailable

An error code that indicates the VPN connection failed because the system isn’t connected to a network.

case unrecoverableNetworkChange

An error code that indicates network conditions changed such that the VPN connection needed to terminate.

case configurationFailed

An error code that indicates the VPN connection failed because the configuration is invalid.

case authenticationFailed

An error code that indicates the VPN connection failed because the VPN server rejected the user credentials.

case configurationNotFound

An error code that indicates the VPN connection failed because the system couldn’t find a configuration.

case negotiationFailed

An error code that indicates the VPN connection failed because the negotiation failed.

### VPN server error codes

case serverAddressResolutionFailed

An error code that indicates the VPN connection failed because the system couldn’t determine the VPN server address.

case serverNotResponding

An error code that indicates the VPN connection failed because the VPN server isn’t responding.

case serverDead

An error code that indicates the VPN connection failed because the VPN server has stopped responding.

case serverDisconnected

An error code that indicates the VPN connection failed because the VPN server terminated the connection.

### Plugin error codes

case pluginFailed

An error code that indicates the VPN plugin failed unexpectedly.

case pluginDisabled

An error code that indicates the VPN plugin isn’t available or needs an update.

### Client certificate error codes

case clientCertificateInvalid

An error code that indicates the client certfiicate is invalid.

case clientCertificateNotYetValid

An error code that indicates the client certfiicate won’t be valid until some time in the future.

case clientCertificateExpired

An error code that indicates the client certfiicate’s validity period has passed.

### Server certificate error codes

case serverCertificateInvalid

An error code that indicates the server certfiicate is invalid.

case serverCertificateNotYetValid

An error code that indicates the server certfiicate won’t be valid until some time in the future.

case serverCertificateExpired

An error code that indicates the server certfiicate’s validity period has passed.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling errors

func fetchLastDisconnectError(completionHandler: ((any Error)?) -> Void)

Retrives the most recent error that caused the VPN to disconnect.

let NEVPNConnectionErrorDomain: String

The domain for errors resulting from VPN connection calls.

