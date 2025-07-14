

- App Store Connect API
-  BetaLicenseAgreementsResponse 

Object

# BetaLicenseAgreementsResponse

A response that contains a list of Beta License Agreement resources.

App Store Connect API 1.0+

``` source
object BetaLicenseAgreementsResponse
```

## Properties

`data`

`[`BetaLicenseAgreement`]`

 (Required) 

The resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

`included`

`[`App`]`

## See Also

### Related Documentation

List Beta License Agreements

Find and list beta license agreements for all apps.

### Objects

object BetaLicenseAgreement

The data structure that represents a Beta License Agreements resource.

object BetaLicenseAgreementUpdateRequest

The request body you use to update a Beta License Agreement.

object BetaLicenseAgreementWithoutIncludesResponse

object BetaLicenseAgreementResponse

A response that contains a single Beta License Agreements resource.

