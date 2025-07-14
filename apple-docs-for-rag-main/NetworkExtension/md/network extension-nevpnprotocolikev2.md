

- Network Extension
-  NEVPNProtocolIKEv2 

Class

# NEVPNProtocolIKEv2

Settings for an IKEv2 VPN configuration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEVPNProtocolIKEv2
```

## Overview

Instances of this class are thread safe.

## Topics

### Accessing IKEv2 Security Association parameters

var ikeSecurityAssociationParameters: NEVPNIKEv2SecurityAssociationParameters

An NEVPNIKEv2SecurityAssociationParameters object containing the parameters for the initial IKE security association to be negotiated with the IKEv2 server.

var childSecurityAssociationParameters: NEVPNIKEv2SecurityAssociationParameters

An NEVPNIKEv2SecurityAssociationParameters object containing the parameters for the child IPSec security associations to be negotiated for each IKEv2 policy.

class NEVPNIKEv2SecurityAssociationParameters

Parameters for an IKEv2 Security Association.

### Accessing certificate properties

var serverCertificateIssuerCommonName: String?

A string containing the value of the Subject Common Name field of the Certificate Authority certificate that issued the IKEv2 server’s certificate.

var serverCertificateCommonName: String?

A string containing the value of the Subject Common Name field of the IKEv2 server’s certificate.

var certificateType: NEVPNIKEv2CertificateType

The type of the certificate in the identity configured in `identityReference` or `identityData`.

enum NEVPNIKEv2CertificateType

An enumeration of certificate type values.

### Accessing TLS version properties

var minimumTLSVersion: NEVPNIKEv2TLSVersion

The minimum TLS version to allow for EAP-TLS authentication.

var maximumTLSVersion: NEVPNIKEv2TLSVersion

The minimum TLS version to allow for EAP-TLS authentication.

enum NEVPNIKEv2TLSVersion

An enumeration of TLS Versions for use in EAP-TLS.

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

var mtu: Int

The Maximum Transmission Unit (MTU) size in bytes to assign to the tunnel interface.

### Supporting Wi-Fi assist

var enableFallback: Bool

A property to enable the use of cellular data when Wi-Fi connectivity is poor.

### Instance Properties

var ppkConfiguration: NEVPNIKEv2PPKConfiguration?

## Relationships

### Inherits From

- NEVPNProtocolIPSec

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### VPN configuration

class NEVPNManager

An object to create and manage a Personal VPN configuration.

class NEVPNProtocolIPSec

Settings for an IPsec VPN configuration.

class NEVPNProtocol

Settings common to both IKEv2 and IPsec VPN configurations.

VPN On Demand Rules

Set up VPN On Demand.

