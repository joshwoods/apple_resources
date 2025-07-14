

- Network Extension
- NEVPNProtocolIKEv2
-  mtu 

Instance Property

# mtu

The Maximum Transmission Unit (MTU) size in bytes to assign to the tunnel interface.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
var mtu: Int { get set }
```

## See Also

### Accessing other IKEv2 properties

var deadPeerDetectionRate: NEVPNIKEv2DeadPeerDetectionRate

The frequency at which the IKEv2 client will run the dead peer detection algorithm.

enum NEVPNIKEv2DeadPeerDetectionRate

An enumeration of values for the frequency at which the IKEv2 client runs the dead peer detection algorithm.

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

