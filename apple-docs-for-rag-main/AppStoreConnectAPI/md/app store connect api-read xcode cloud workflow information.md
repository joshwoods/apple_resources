

- App Store Connect API
-  Read Xcode Cloud Workflow Information 

Web Service Endpoint

# Read Xcode Cloud Workflow Information

Get information about a specific Xcode Cloud workflow.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciWorkflows/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Workflows resource.

## Query Parameters

`fields[ciWorkflows]`

`[string]`

Additional fields to include for the Workflows resource returned by the response.

Possible Values: `name, description, branchStartCondition, tagStartCondition, pullRequestStartCondition, scheduledStartCondition, manualBranchStartCondition, manualTagStartCondition, manualPullRequestStartCondition, actions, isEnabled, isLockedForEditing, clean, containerFilePath, lastModifiedDate, product, repository, xcodeVersion, macOsVersion, buildRuns`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `product, repository, xcodeVersion, macOsVersion`

`fields[scmRepositories]`

`[string]`

Additional fields to include for the Workflows resource returned by the response.

Possible Values: `lastAccessedDate, httpCloneUrl, sshCloneUrl, ownerName, repositoryName, scmProvider, defaultBranch, gitReferences, pullRequests`

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

## Discussion

The example request below accesses information about an Xcode Cloud workflow. Display the workflow data provided in the response on a dashboard or use it to read additional information; for example, detailed data about builds Xcode Cloud performed.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f
```

```
{
    "data": {
        "type": "ciWorkflows",
        "id": "3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f",
        "attributes": {
            "name": "My Workflow",
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
            "product": {
                "data": {
                    "type": "ciProducts",
                    "id": "8ca28eb1-2948-4848-813b-07c500665157"
                }
            },
            "repository": {
                "data": {
                    "type": "scmRepositories",
                    "id": "195430ae-7262-4b24-abd2-cbb6891feab8"
                },
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f/relationships/repository",
                    "related": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f/repository"
                }
            },
            "xcodeVersion": {
                "data": {
                    "type": "ciXcodeVersions",
                    "id": "Xcode12E507:stable"
                }
            },
            "macOsVersion": {
                "data": {
                    "type": "ciMacOsVersions",
                    "id": "20G95"
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
        "self": "https://api.appstoreconnect.apple.com/v1/ciWorkflows/3fa0575f-4de0-44cb-bf0f-9aa2651c2f1f?include=macOsVersion%2Cproduct%2Crepository%2CxcodeVersion"
    }
}
```

## See Also

### Getting Xcode Cloud Workflows

List All Xcode Cloud Builds for a Workflow

List all builds Xcode Cloud performed for a specific workflow.

Read the Repository Information for an Xcode Cloud Workflow

Get information about the Git repository of a specific Xcode Cloud workflow.

