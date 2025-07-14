

- Enterprise Program API
-  Create a PassTypeId 

Web Service Endpoint

# Create a PassTypeId

Create a new identifier for use with a pass type ID certificate using a certificate signing request.

## URL

``` source
POST https://api.enterprise.developer.apple.com/v1/passTypeIds
```

## HTTP Body

PassTypeIdCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

PassTypeIdResponse

`Created`

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

List Pass Type Ids

Find and list pass type IDs that are registered to your team.

Read PassTypeId Information

Get information about a specific pass type ID.

List All Certificates for a PassTypeId

List all certificates for a specific pass type ID.

Modify a PassTypeId

Update a specific pass type ID’s name.

Delete a PassTypeId

Delete a pass type ID that is used for app development.

