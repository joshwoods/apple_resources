

- Network Extension
- NEVPNProtocolIKEv2
-  serverCertificateCommonName 

Instance Property

# serverCertificateCommonName

A string containing the value of the Subject Common Name field of the IKEv2 server’s certificate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var serverCertificateCommonName: String? { get set }
```

## Discussion

This string is used to help verify the identity of the IKEv2 server.

## See Also

### Accessing certificate properties

var serverCertificateIssuerCommonName: String?

A string containing the value of the Subject Common Name field of the Certificate Authority certificate that issued the IKEv2 server’s certificate.

var certificateType: NEVPNIKEv2CertificateType

The type of the certificate in the identity configured in `identityReference` or `identityData`.

enum NEVPNIKEv2CertificateType

An enumeration of certificate type values.

