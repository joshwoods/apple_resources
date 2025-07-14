

- Network Extension
-  NEVPNIKEv2DeadPeerDetectionRate 

Enumeration

# NEVPNIKEv2DeadPeerDetectionRate

An enumeration of values for the frequency at which the IKEv2 client runs the dead peer detection algorithm.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
enum NEVPNIKEv2DeadPeerDetectionRate
```

## Topics

### Detection rates

case none

Do not perform dead peer detection.

case low

Run dead peer detection once every 30 minutes. If the peer does not respond, retry 5 times at 1 second intervals before declaring the peer dead and terminating the session.

case medium

Run dead peer detection once every 10 minutes. If the peer does not respond, retry 5 times at 1 second intervals before declaring the peer dead and terminating the session.

case high

Run dead peer detection once every 1 minute. If the peer does not respond, retry 5 times at 1 second intervals before declaring the peer dead and terminating the session.

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

### Accessing other IKEv2 properties

var deadPeerDetectionRate: NEVPNIKEv2DeadPeerDetectionRate

The frequency at which the IKEv2 client will run the dead peer detection algorithm.

var useConfigurationAttributeInternalIPSubnet: Bool

A Boolean indicating whether or not the IKEv2 client should use the INTERNAL_IP4_SUBNET and/or INTERNAL_IP6_SUBNET attributes sent by the IKEv2 server.

var disableMOBIKE: Bool

A Boolean indicating whether or not MOBIKE should be disabled for the IKEv2 sessions.

var disableRedirect: Bool

A Boolean indicating whether or not IKEv2 server redirects are disabled.

var enablePFS: Bool

A Boolean indicating whether or not Perfect Forward Secrecy is enabled.

var enableRevocationCheck: Bool

Enable revocation checking of the IKEv2 server certificate.

var strictRevocationCheck: Bool

Require a “not revoked” result when checking if the certificate identifying the server is revoked.

var mtu: Int

The Maximum Transmission Unit (MTU) size in bytes to assign to the tunnel interface.

