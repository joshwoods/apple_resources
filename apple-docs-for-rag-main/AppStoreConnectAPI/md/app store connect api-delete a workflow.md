

- App Store Connect API
-  Delete a Workflow 

Web Service Endpoint

# Delete a Workflow

Delete an Xcode Cloud workflow and all of its associated data.

App Store Connect API 1.5+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/ciWorkflows/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Workflows resource.

## Response Codes

` 204 ``No Content`

`No Content`

The request completed successfully and the specific Workflows resource was deleted.

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

To delete an Xcode Cloud workflow, call this endpoint using the HTTP `DELETE` method like this:

```
```

App Store Connect confirms the deletion by responding with the `HTTP/1.1 204 No Content` HTTP status code.

Important

Deleting an Xcode Cloud workflow permanently deletes its build history and artifacts. Only delete an Xcode Cloud workflow when you’re confident that you no longer need it and its build history or artifacts. Instead of deleting a workflow, deactivate it to preserve its build history and artifacts. To deactivate a workflow, use the Update an Xcode Cloud Workflow endpoint to set the workflow’s `isEnabled` attribute to `false` or deactivate it in the Xcode or App Store Connect. For more information about deactivating a workflow using Xcode or App Store Connect, see Developing a workflow strategy for Xcode Cloud.

## See Also

### Managing Xcode Cloud Workflows

Create a Workflow

Create a new Xcode Cloud workflow for an Xcode Cloud product.

Update an Xcode Cloud Workflow

Make changes to an Xcode Cloud workflow.

