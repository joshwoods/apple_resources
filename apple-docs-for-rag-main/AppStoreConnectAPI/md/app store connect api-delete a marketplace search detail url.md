

- App Store Connect API
-  Delete a marketplace search detail URL 

Web Service Endpoint

# Delete a marketplace search detail URL

Delete search detail URL for the alternative marketplace.

App Store Connect API 3.3+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/marketplaceSearchDetails/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `marketplace search details` resource ID from the Read the marketplace search detail URL response.

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

## Discussion

### Example Request and Response

- Request
- Response

```
DELETE https://api.appstoreconnect.apple.com/v1/marketplaceSearchDetails/{id}
```

```
204
```

## See Also

### Managing search URLs

Building a searchable catalog for your marketplace app for inclusion in Spotlight

Set up and build your alternative marketplace’s searchable index.

Add a marketplace search detail URL

Add a search detail URL for the alternative marketplace.

Read the marketplace search detail URL

Get search detail URL for the alternative marketplace.

Modify a marketplace search detail URL

Update the search detail URL for the alternative marketplace.

