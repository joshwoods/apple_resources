

- App Store Connect API
-  Update an Xcode Cloud Workflow 

Web Service Endpoint

# Update an Xcode Cloud Workflow

Make changes to an Xcode Cloud workflow.

App Store Connect API 1.5+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/ciWorkflows/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Workflows resource.

## HTTP Body

CiWorkflowUpdateRequest

The request body you use to update an Xcode Cloud workflow.

Content-Type: application/json

## Response Codes

` 200 ``OK`

CiWorkflowResponse

`OK`

The request completed successfully.

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

The example request below updates the name of an existing Xcode Cloud workflow. For a successful update, the response includes detailed information about the workflow. Use it to access additional information, start a new build, and so on.

### Example Request and Response

- Request
- Response

```
PATCH https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f

{
    "data": {
        "type": "ciWorkflows",
        "id": "3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f",
        "attributes": {
            "name": "A new name for an existing workflow."
        }
    }
}
```

```
{
    "data": {
        "type": "ciWorkflows",
        "id": "3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f",
        "attributes": {
            "name": "A new name for an existing workflow.",
            "description": "",
            "branchStartCondition": {
                "source": {
                    "isAllMatch": false,
                    "patterns": [
                        {
                            "pattern": "main",
                            "isPrefix": false
                        }
                    ]
                },
                "filesAndFoldersRule": {
                    "mode": "START_IF_ANY_FILE_MATCHES",
                    "matchers": []
                },
                "autoCancel": true
            },
            "tagStartCondition": null,
            "pullRequestStartCondition": null,
            "scheduledStartCondition": null,
            "actions": [
                {
                    "name": "Archive iOS",
                    "actionType": "ARCHIVE",
                    "destination": null,
                    "buildDistributionAudience": null,
                    "testConfiguration": null,
                    "scheme": "MyApp",
                    "platform": "IOS",
                    "isRequiredToPass": true
                }
            ],
            "isEnabled": true,
            "isLockedForEditing": false,
            "clean": false,
            "containerFilePath": "MyXcodeProject.xcodeproj",
            "lastModifiedDate": null
        },
        "relationships": {
            "repository": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f/relationships/repository",
                    "related": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f/repository"
                }
            },
            "buildRuns": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f/relationships/buildRuns",
                    "related": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f/buildRuns"
                }
            }
        },
        "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f"
        }
    },
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f"
    }
}
```

## See Also

### Managing Xcode Cloud Workflows

Create a Workflow

Create a new Xcode Cloud workflow for an Xcode Cloud product.

Delete a Workflow

Delete an Xcode Cloud workflow and all of its associated data.

