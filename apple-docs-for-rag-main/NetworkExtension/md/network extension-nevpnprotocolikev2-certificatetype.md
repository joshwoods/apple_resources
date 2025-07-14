

- Network Extension
- NEVPNProtocolIKEv2
-  certificateType 

Instance Property

# certificateType

The type of the certificate in the identity configured in `identityReference` or `identityData`.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var certificateType: NEVPNIKEv2CertificateType { get set }
```

## Discussion

The default value is NEVPNIKEv2CertificateType.RSA.

## See Also

### Accessing certificate properties

var serverCertificateIssuerCommonName: String?

A string containing the value of the Subject Common Name field of the Certificate Authority certificate that issued the IKEv2 server’s certificate.

var serverCertificateCommonName: String?

A string containing the value of the Subject Common Name field of the IKEv2 server’s certificate.

enum NEVPNIKEv2CertificateType

An enumeration of certificate type values.

