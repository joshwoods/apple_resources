

- App Store Connect API
-  Get All App Resource IDs for a Beta Tester 

Web Service Endpoint

# Get All App Resource IDs for a Beta Tester

Get a list of app resource IDs associated with a beta tester.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaTesters/{id}/relationships/apps
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

BetaTesterAppsLinkagesResponse

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

### Reading Beta Tester Details

List All Apps for a Beta Tester

Get a list of apps that a beta tester can test.

List All Builds Individually Assigned to a Beta Tester

Get a list of builds individually assigned to a specific beta tester.

Get All IDs of Builds Individually Assigned to a Beta Tester

Get a list of build resource IDs individually assigned to a specific beta tester.

List All Beta Groups to Which a Beta Tester Belongs

Get a list of beta groups that contain a specific beta tester.

Get All Beta Group IDs of a Beta Tester's Groups

Get a list of group resource IDs associated with a beta tester.

