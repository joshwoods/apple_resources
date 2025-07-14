

- Enterprise Program API
-  Modify a PassTypeId 

Web Service Endpoint

# Modify a PassTypeId

Update a specific pass type ID’s name.

## URL

``` source
PATCH https://api.enterprise.developer.apple.com/v1/passTypeIds/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

PassTypeIdUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

PassTypeIdResponse

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Overview

- HTTPBody

## See Also

### Managing Pass Type Ids

Create a PassTypeId

Create a new identifier for use with a pass type ID certificate using a certificate signing request.

List Pass Type Ids

Find and list pass type IDs that are registered to your team.

Read PassTypeId Information

Get information about a specific pass type ID.

List All Certificates for a PassTypeId

List all certificates for a specific pass type ID.

Delete a PassTypeId

Delete a pass type ID that is used for app development.

