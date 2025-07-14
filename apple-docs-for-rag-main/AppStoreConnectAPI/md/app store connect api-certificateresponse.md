

- App Store Connect API
-  CertificateResponse 

Object

# CertificateResponse

A response that contains a single Certificates resource.

App Store Connect API 1.1+

``` source
object CertificateResponse
```

## Properties

`data`

Certificate

 (Required) 

The resource data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

## See Also

### Related Documentation

Create a Certificate

Create a new certificate using a certificate signing request.

### Object and data types

object Certificate

The data structure that represents a Certificates resource.

object CertificatesWithoutIncludesResponse

object CertificateCreateRequest

The request body you use to create a Certificate.

object CertificatesResponse

A response that contains a list of Certificates resources.

object CertificateUpdateRequest

The request body you use to update a certificate activation status.

type CertificateType

Literal values that represent types of signing certificates.

