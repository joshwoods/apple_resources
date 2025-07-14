

- Enterprise Program API
-  CertificatesResponse 

Object

# CertificatesResponse

A response that contains a list of Certificates resources.

``` source
object CertificatesResponse
```

## Properties

`data`

`[`Certificate`]`

 (Required) 

The resource data.

`included`

`[`PassTypeId`]`

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information

## Attributes 

Possible types:

## See Also

### Object and Data Types

object Certificate

The data structure that represents a Certificates resource.

object CertificatesWithoutIncludesResponse

A response that contains a single certificate resource without includes.

object CertificateCreateRequest

The request body you use to create a Certificate.

object CertificateResponse

A response that contains a single Certificates resource.

type CertificateType

Literal values that represent types of signing certificates.

