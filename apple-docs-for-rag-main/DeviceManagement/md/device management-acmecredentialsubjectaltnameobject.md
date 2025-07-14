

- Device Management
-  ACMECredentialSubjectAltNameObject 

Object

# ACMECredentialSubjectAltNameObject

Specifies the subject’s alternative name that the device requests for the certificate that the ACME server issues.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ACMECredentialSubjectAltNameObject
```

## Properties

`dNSName`

`string`

The DNS name.

`ntPrincipalName`

`string`

The NT principal name.

`rfc822Name`

`string`

The RFC 822 email address.

`uniformResourceIdentifier`

`string`

The uniform resource identifier.

## Discussion

The ACME server may override or ignore this field in the certificate it issues.

