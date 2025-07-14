

- Enterprise Program API
-  List All Certificates for a PassTypeId 

Web Service Endpoint

# List All Certificates for a PassTypeId

List all certificates for a specific pass type ID.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/passTypeIds/{id}/certificates
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[certificates]`

`[string]`

Possible Values: `certificateContent, certificateType, csrContent, displayName, expirationDate, name, passTypeId, platform, serialNumber`

`fields[passTypeIds]`

`[string]`

Possible Values: `certificates, identifier, name`

`filter[certificateType]`

`[string]`

Possible Values: `IOS_DEVELOPMENT, IOS_DISTRIBUTION, MAC_APP_DISTRIBUTION, MAC_INSTALLER_DISTRIBUTION, MAC_APP_DEVELOPMENT, DEVELOPER_ID_KEXT, DEVELOPER_ID_APPLICATION, DEVELOPMENT, DISTRIBUTION, PASS_TYPE_ID, PASS_TYPE_ID_WITH_NFC`

`filter[displayName]`

`[string]`

`filter[id]`

`[string]`

`filter[serialNumber]`

`[string]`

`include`

`[string]`

Value: `passTypeId`

`limit`

`integer`

Maximum: `200`

`sort`

`[string]`

Possible Values: `certificateType, -certificateType, displayName, -displayName, id, -id, serialNumber, -serialNumber`

## Response Codes

` 200 ``OK`

CertificatesResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## See Also

### Managing Pass Type Ids

Create a PassTypeId

Create a new identifier for use with a pass type ID certificate using a certificate signing request.

List Pass Type Ids

Find and list pass type IDs that are registered to your team.

Read PassTypeId Information

Get information about a specific pass type ID.

Modify a PassTypeId

Update a specific pass type ID’s name.

Delete a PassTypeId

Delete a pass type ID that is used for app development.

