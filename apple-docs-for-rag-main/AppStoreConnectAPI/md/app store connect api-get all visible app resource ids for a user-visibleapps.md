

- App Store Connect API
-  Get All Visible App Resource IDs for a User 

Web Service Endpoint

# Get All Visible App Resource IDs for a User

Get a list of app resource IDs to which a user on your team has access.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/users/{id}/relationships/visibleApps
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

UserVisibleAppsLinkagesResponse

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

### Listing, Adding, and Removing App Access

List All Apps Visible to a User

Get a list of apps that a user on your team can view.

Add Visible Apps to a User

Give a user on your team access to one or more apps.

Replace the List of Visible Apps for a User

Replace the list of apps a user on your team can see.

Remove Visible Apps from a User

Remove a user on your team’s access to one or more apps.

