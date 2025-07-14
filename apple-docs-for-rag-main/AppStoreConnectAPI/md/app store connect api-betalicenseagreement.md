

- App Store Connect API
-  BetaLicenseAgreement 

Object

# BetaLicenseAgreement

The data structure that represents a Beta License Agreements resource.

App Store Connect API 1.0+

``` source
object BetaLicenseAgreement
```

## Properties

`attributes`

BetaLicenseAgreement.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

BetaLicenseAgreement.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `betaLicenseAgreements`

## Topics

### Objects

object BetaLicenseAgreement.Attributes

Attributes that describe a Beta License Agreements resource.

object BetaLicenseAgreement.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object BetaLicenseAgreementUpdateRequest

The request body you use to update a Beta License Agreement.

object BetaLicenseAgreementWithoutIncludesResponse

object BetaLicenseAgreementsResponse

A response that contains a list of Beta License Agreement resources.

object BetaLicenseAgreementResponse

A response that contains a single Beta License Agreements resource.

