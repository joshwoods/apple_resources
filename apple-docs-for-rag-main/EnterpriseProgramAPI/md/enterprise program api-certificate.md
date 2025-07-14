

- Enterprise Program API
-  Certificate 

Object

# Certificate

The data structure that represents a Certificates resource.

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

`relationships`

Certificate.Relationships

## Attributes 

Possible types:

## Topics

### Objects

object Certificate.Attributes

Attributes that describe a Certificates resource.

object Certificate.Relationships

The data and links that describe the relationship between the resources.

## See Also

### Object and Data Types

object CertificatesWithoutIncludesResponse

A response that contains a single certificate resource without includes.

object CertificateCreateRequest

The request body you use to create a Certificate.

object CertificateResponse

A response that contains a single Certificates resource.

object CertificatesResponse

A response that contains a list of Certificates resources.

type CertificateType

Literal values that represent types of signing certificates.

