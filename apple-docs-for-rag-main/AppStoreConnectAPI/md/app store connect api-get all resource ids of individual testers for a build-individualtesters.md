

- App Store Connect API
-  Get All Resource IDs of Individual Testers for a Build 

Web Service Endpoint

# Get All Resource IDs of Individual Testers for a Build

Get a list of resource IDs of individual testers associated with a build.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/builds/{id}/relationships/individualTesters
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`limit`

`integer`

Number of resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

BuildIndividualTestersLinkagesResponse

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

Resource not found.

Content-Type: application/json

## See Also

### Listing Individually Assigned Beta Testers

List All Individual Testers for a Build

Get a list of beta testers individually assigned to a build.

