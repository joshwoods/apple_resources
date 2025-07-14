

- Enterprise Program API
-  CertificateResponse 

Object

# CertificateResponse

A response that contains a single Certificates resource.

``` source
object CertificateResponse
```

## Properties

`data`

Certificate

 (Required) 

The resource data.

`included`

`[`PassTypeId`]`

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

## Attributes 

Possible types:

## Topics

### Related Documentation

Create a Certificate

Create a new certificate using a certificate signing request.

## See Also

### Object and Data Types

object Certificate

The data structure that represents a Certificates resource.

object CertificatesWithoutIncludesResponse

A response that contains a single certificate resource without includes.

object CertificateCreateRequest

The request body you use to create a Certificate.

object CertificatesResponse

A response that contains a list of Certificates resources.

type CertificateType

Literal values that represent types of signing certificates.

