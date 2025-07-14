

- Device Management
-  VppServiceConfigResponse 

Object

# VppServiceConfigResponse

The response with the service configuration.

Device Assignment ServicesVPP License Management

``` source
object VppServiceConfigResponse
```

## Properties

`associateLicenseSrvUrl`

`string`

The URL for the `Associate License` endpoint. Note the `Associate License` endpoint has been deprecated. Use Manage Licenses instead.

`clientConfigSrvUrl`

`string`

The URL for the Client Configuration endpoint.

`contentMetadataLookupUrl`

`string`

The URL that returns metadata about a product in the iTunes Store.

See Getting App and Book Information (Legacy), for more information.

`disassociateLicenseSrvUrl`

`string`

The URL for the `Disassociate License` endpoint. Note the `Disassociate License` endpoint has been deprecated. Use Manage Licenses instead.

`editUserSrvUrl`

`string`

The URL for the Edit a User endpoint.

`errorCodes`

VppErrorCode

List of possible error numbers and their human-readable explanations.

`errorMessage`

`string`

The human-readable explanation of the error.

`errorNumber`

`int32`

The numeric code of the error.

`getLicensesSrvUrl`

`string`

The URL for the Get Licenses endpoint.

`getUserSrvUrl`

`string`

The URL for the Get a User endpoint.

`getUsersSrvUrl`

`string`

The URL for the Get Users endpoint.

`getVPPAssetsSrvUrl`

`string`

The URL for the Get Assets endpoint.

`invitationEmailUrl`

`string`

The URL template for inviting users to an organization.

`manageVPPLicensesByAdamIdSrvUrl`

`string`

The URL for the Manage Licenses endpoint.

`maxBatchAssociateLicenseCount`

`int32`

The maximum number of entries allowed in the arrays for associating licenses with Manage Licenses. The MDM server should check this value every 5 minutes, because it could change without notice.

`maxBatchDisassociateLicenseCount`

`int32`

The maximum number of entries allowed in the arrays for disassociating licenses from Manage Licenses. The MDM server should check this value every 5 minutes, because it could change without notice.

`registerUserSrvUrl`

`string`

The URL for the Register a User endpoint.

`retireUserSrvUrl`

`string`

The URL for the Retire a User endpoint.

`status`

`int32`

The status code for the response. Possible values are:

`0` = Success. `-1` = Failure.

`vppWebsiteUrl`

`string`

The URL for the VPP website.

