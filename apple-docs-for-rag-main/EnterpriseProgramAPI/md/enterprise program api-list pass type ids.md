

- Enterprise Program API
-  List Pass Type Ids 

Web Service Endpoint

# List Pass Type Ids

Find and list pass type IDs that are registered to your team.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/passTypeIds
```

## Query Parameters

`fields[certificates]`

`[string]`

Possible Values: `certificateContent, certificateType, csrContent, displayName, expirationDate, name, passTypeId, platform, serialNumber`

`fields[passTypeIds]`

`[string]`

Possible Values: `certificates, identifier, name`

`filter[id]`

`[string]`

`filter[identifier]`

`[string]`

`filter[name]`

`[string]`

`include`

`[string]`

Value: `certificates`

`limit`

`integer`

Maximum: `200`

`limit[certificates]`

`integer`

Maximum: `50`

`sort`

`[string]`

Possible Values: `id, -id, identifier, -identifier, name, -name`

## Response Codes

` 200 ``OK`

PassTypeIdsResponse

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

## See Also

### Managing Pass Type Ids

Create a PassTypeId

Create a new identifier for use with a pass type ID certificate using a certificate signing request.

Read PassTypeId Information

Get information about a specific pass type ID.

List All Certificates for a PassTypeId

List all certificates for a specific pass type ID.

Modify a PassTypeId

Update a specific pass type ID’s name.

Delete a PassTypeId

Delete a pass type ID that is used for app development.

