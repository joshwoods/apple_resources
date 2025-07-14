

- Device Management
-  GetVppAssetRequest 

Object

# GetVppAssetRequest

The request for an asset.

Device Assignment ServicesVPP License Management

``` source
object GetVppAssetRequest
```

## Properties

`includeLicenseCounts`

`boolean`

If `true`, returns the total number of licenses, the number of assigned licenses, and the number of unassigned licenses in the response for each asset.

`pricingParam`

`string`

The quality of a product in the iTunes Store. If a pricing parameter is specified, only records with that parameter are included in the results. Possible values are:

- `STDQ`: Standard quality

- `PLUS`: High quality

`sToken`

`string`

 (Required) 

The authentication token. For more information, see Authentication.

## See Also

### Request and Response

object GetVppAssetResponse

The response with the asset.

