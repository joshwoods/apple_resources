

- App Store Connect API
-  Delete a Product 

Web Service Endpoint

# Delete a Product

Delete an Xcode Cloud product and all of its associated workflows, builds, and artifacts.

App Store Connect API 1.5+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/ciProducts/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Products resource.

## Response Codes

` 204 ``No Content`

`No Content`

The request completed successfully and the specific Products resource was deleted.

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

## Discussion

To delete an Xcode Cloud product, call this endpoint using the HTTP `DELETE` method like this:

```
https://api.appstoreconnect.apple.com/v1/ciProducts/9ad354b0-f380-40d3-b94f-dd5225b8b3d5
```

App Store Connect confirms the deletion by responding with the `HTTP/1.1 204 No Content` HTTP status code.

Important

Deleting an Xcode Cloud product permanently deletes all workflows, including their build history and artifacts. Only delete an Xcode Cloud product when you’re confident that you don’t need its workflows, build history, or artifacts anymore. Instead of deleting a product, deactivate its workflows to preserve the product and its build history and artifacts. For more information about deactivating a workflow, see Developing a workflow strategy for Xcode Cloud.

