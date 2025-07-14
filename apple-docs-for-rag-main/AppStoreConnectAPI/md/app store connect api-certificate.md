

- App Store Connect API
-  Certificate 

Object

# Certificate

The data structure that represents a Certificates resource.

App Store Connect API 1.1+

``` source
object Certificate
```

## Properties

`attributes`

Certificate.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`type`

`string`

 (Required) 

The resource type.

Value: `certificates`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object Certificate.Attributes

Attributes that describe a Certificates resource.

## See Also

### Object and data types

object CertificatesWithoutIncludesResponse

object CertificateCreateRequest

The request body you use to create a Certificate.

object CertificateResponse

A response that contains a single Certificates resource.

object CertificatesResponse

A response that contains a list of Certificates resources.

object CertificateUpdateRequest

The request body you use to update a certificate activation status.

type CertificateType

Literal values that represent types of signing certificates.

