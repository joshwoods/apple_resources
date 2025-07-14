

- App Store Connect API
-  Modify the Build for an App Store Version 

Web Service Endpoint

# Modify the Build for an App Store Version

Change the build that is attached to a specific App Store version.

App Store Connect API 1.2+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/relationships/build
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

AppStoreVersionBuildLinkageRequest

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

## Discussion

Use this endpoint to associate a build with a version. The build you specify represents the build that’s installed when a customer purchases the app on the App Store.

### Attach a Build to a Version

- Request
- Response

```
PATCH https://api.appstoreconnect.apple.com/v1/appStoreVersions/f5b10fc0-afda-4b31-b3e8-cdbcbe945622/relationships/build
{
  "data": {
    "type": "builds",
    "id": "b539f38f-8af4-4fbd-b5fc-fde89aab410f"
  }
}

```

```
{
  "data": {
    "type": "builds",
    "id": "b539f38f-8af4-4fbd-b5fc-fde89aab410f"
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/f5b10fc0-afda-4b31-b3e8-cdbcbe945622/relationships/build",
    "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/f5b10fc0-afda-4b31-b3e8-cdbcbe945622/build"
  }
}
```

### Remove the Build from a Version

- Request
- Response

```
PATCH /v1/appStoreVersions/f5b10fc0-afda-4b31-b3e8-cdbcbe945622/relationships/build
{
  "data": null
}
```

```
{
  "data": null,
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/f5b10fc0-afda-4b31-b3e8-cdbcbe945622/relationships/build",
    "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/f5b10fc0-afda-4b31-b3e8-cdbcbe945622/build"
  }
}
```

## See Also

### Attaching a Build to a Version

Read the Build Information of an App Store Version

Get the build that is attached to a specific App Store version.

Get the Build ID for an App Store Version

Get the ID of the build that is attached to a specific App Store version.

