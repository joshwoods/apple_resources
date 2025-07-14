

- App Store Connect API
-  Delete a featuring nomination 

Web Service Endpoint

# Delete a featuring nomination

Remove a specific featuring nomination.

App Store Connect API 3.8+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/nominations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

## Overview

- id: An opaque resource ID that uniquely identifies the resource. Obtain the nomination resource ID from the List nominations response.

## See Also

### Managing nominations

Create a featuring nomination

Tell Apple about your upcoming app or feature.

List nominations

Get all featuring nominations.

Read details for a nomination

Get information for a specific featuring nomination.

Modify a nomination

Update a specific featuring nomination.

