

- Network Extension
- NEVPNProtocolIKEv2
-  strictRevocationCheck 

Instance Property

# strictRevocationCheck

Require a “not revoked” result when checking if the certificate identifying the server is revoked.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var strictRevocationCheck: Bool { get set }
```

## Discussion

The default value is NO. If this property is set to NO, then either a “not revoked” result from the certificate revocation server or a failure to communicate with the certificate revocation server will result in a successful revocation check. If this property is set to YES, then only a “not revoked” result from the certificate revocation server will result in a successful revocation check.

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

var mtu: Int

The Maximum Transmission Unit (MTU) size in bytes to assign to the tunnel interface.

