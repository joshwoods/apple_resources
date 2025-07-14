

- App Store Connect API
-  CertificatesResponse 

Object

# CertificatesResponse

A response that contains a list of Certificates resources.

App Store Connect API 1.1+

``` source
object CertificatesResponse
```

## Properties

`data`

`[`Certificate`]`

 (Required) 

The resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information

## See Also

### Related Documentation

List and Download Certificates

Find and list certificates and download their data.

### Object and data types

object Certificate

The data structure that represents a Certificates resource.

object CertificatesWithoutIncludesResponse

object CertificateCreateRequest

The request body you use to create a Certificate.

object CertificateResponse

A response that contains a single Certificates resource.

object CertificateUpdateRequest

The request body you use to update a certificate activation status.

type CertificateType

Literal values that represent types of signing certificates.

