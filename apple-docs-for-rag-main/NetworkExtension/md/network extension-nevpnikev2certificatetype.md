

- Network Extension
-  NEVPNIKEv2CertificateType 

Enumeration

# NEVPNIKEv2CertificateType

An enumeration of certificate type values.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
enum NEVPNIKEv2CertificateType
```

## Topics

### Certificate types

case RSA

The RSA certificate type.

case ECDSA256

The ECDSA with p-256 curve certificate type.

case ECDSA384

The ECDSA with p-384 curve certificate type.

case ECDSA521

The ECDSA with p-521 curve certificate type.

case ed25519

The Edwards 25519 curve certificate type.

case RSAPSS

The RSA-PSS certificate type.

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

### Accessing certificate properties

var serverCertificateIssuerCommonName: String?

A string containing the value of the Subject Common Name field of the Certificate Authority certificate that issued the IKEv2 server’s certificate.

var serverCertificateCommonName: String?

A string containing the value of the Subject Common Name field of the IKEv2 server’s certificate.

var certificateType: NEVPNIKEv2CertificateType

The type of the certificate in the identity configured in `identityReference` or `identityData`.

