

- App Store Connect API
-  Add Visible Apps to a User 

Web Service Endpoint

# Add Visible Apps to a User

Give a user on your team access to one or more apps.

App Store Connect API 1.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/users/{id}/relationships/visibleApps
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## HTTP Body

UserVisibleAppsLinkagesRequest

Content-Type: application/json

## Response Codes

` 204 ``No Content`

`No Content`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Listing, Adding, and Removing App Access

List All Apps Visible to a User

Get a list of apps that a user on your team can view.

Get All Visible App Resource IDs for a User

Get a list of app resource IDs to which a user on your team has access.

Replace the List of Visible Apps for a User

Replace the list of apps a user on your team can see.

Remove Visible Apps from a User

Remove a user on your team’s access to one or more apps.

