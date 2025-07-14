

- Device Management
- CertificateListResponse
-  CertificateListResponse.CertificateListItem 

Device Management Command

# CertificateListResponse.CertificateListItem

A dictionary that contains information about a certificate list item.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object CertificateListResponse.CertificateListItem
```

## Properties

`CommonName`

`string`

 (Required) 

The certificate’s common name.

`Data`

`data`

 (Required) 

The certificate in DER-encoded X.509 format.

`IsIdentity`

`boolean`

 (Required) 

If `true`, this is an identity certificate.

## See Also

### Commands

object CertificateListResponse.ErrorChainItem

A dictionary that describes an error chain item.

