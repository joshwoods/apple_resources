

- App Store Connect API
-  Create a Workflow 

Web Service Endpoint

# Create a Workflow

Create a new Xcode Cloud workflow for an Xcode Cloud product.

App Store Connect API 1.5+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/ciWorkflows
```

## HTTP Body

CiWorkflowCreateRequest

The request body you use to create a new Xcode Cloud workflow.

Content-Type: application/json

## Response Codes

` 201 ``Created`

CiWorkflowResponse

`Created`

The request completed successfully and a new Workflows resource has been created.

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

The example request below creates a new workflow that performs the archive action. App Store Connect returns the `201` HTTP status code to indicate the successful creation of the workflow and returns information about the workflow. Use the data to access additional information or to start a new build.

### Example Request and Response

- Request
- Response

```
{    
“data”: {
        “type”: “ciWorkflows”,
        “attributes”: {
            “name”: “A new workflow”,
            “description”: “A new workflow that verifies my changes.”,
            “branchStartCondition”: {
                “source”: {
                    “isAllMatch”: false,
                    “patterns”: [
                        {
                            “pattern”: “main”,
                            “isPrefix”: false
                        }
                    ]
                },
                “filesAndFoldersRule”: {
                    “mode”: “START_IF_ANY_FILE_MATCHES”,
                    “matchers”: []
                },
                “autoCancel”: true
            },
            “actions”: [
                {
                    “name”: “Archive iOS”,
                    “actionType”: “ARCHIVE”,
                    “scheme”: “MyApp”,
                    “platform”: “IOS”,
                    “isRequiredToPass”: true
                }
            ],
            “isEnabled”: true,
            “isLockedForEditing”: false,
            “clean”: false,
            “containerFilePath”: “MyXcodeProject.xcodeproj”
        },
        “relationships”: {
            “xcodeVersion”: {
                “data”: {
                    “type”: “ciXcodeVersions”,
                    “id”: “Xcode12E507:stable”
                }
            },
            “macOsVersion”: {
                “data”: {
                    “type”: “ciMacOsVersions”,
                    “id”: “20G95”
                }
            },
            “product”: {
                “data”: {
                    “type”: “ciProducts”,
                    “id”: “8ca28eb1-2948-4848-813b-07c500665157”
                }
            },
            “repository”: {
                “data”: {
                    “type”: “scmRepositories”,
                    “id”: “195430ae-7262-4b24-abd2-cbb6891feab8”
                }
            }
        }
    }
}
```

```
{
    "data": {
        "type": "ciWorkflows",
        "id": "f445a31a-b0c6-4a83-b295-25496f50a69e",
        "attributes": {
            "name": "A new workflow",
            "description": "A new workflow that verifies my changes.",
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
                    "self": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/f445a31a-b0c6-4a83-b295-25496f50a69e/relationships/repository",
                    "related": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/f445a31a-b0c6-4a83-b295-25496f50a69e/repository"
                }
            },
            "buildRuns": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/f445a31a-b0c6-4a83-b295-25496f50a69e/relationships/buildRuns",
                    "related": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/f445a31a-b0c6-4a83-b295-25496f50a69e/buildRuns"
                }
            }
        },
        "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/f445a31a-b0c6-4a83-b295-25496f50a69e"
        }
    },
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciWorkflows"
    }
}
```

## See Also

### Managing Xcode Cloud Workflows

Update an Xcode Cloud Workflow

Make changes to an Xcode Cloud workflow.

Delete a Workflow

Delete an Xcode Cloud workflow and all of its associated data.

