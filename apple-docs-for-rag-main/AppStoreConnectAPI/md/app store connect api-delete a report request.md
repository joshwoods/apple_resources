

- App Store Connect API
-  Delete a report request 

Web Service Endpoint

# Delete a report request

Remove a specific analytics report request.

App Store Connect API 3.4+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Apps resource. Obtain the app resource ID from the Read report requests response.

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

## Mentioned in 

Downloading Analytics Reports

## Discussion

### Examples Request and Response

- Request
- Response

```
DELETE https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231

```

```
204 No Content
```

## See Also

### Making, Reading, and Deleting Requests

Request reports

Request analytics reports for your apps.

Read report requests

Read analytics report requests for a specific app.

Read report request information

Get details for and the state of a specific analytics report request.

Read reports for a specific request

Get a list of reports generated from a specific analytics report request.

