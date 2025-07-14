

- App Store Connect API
-  List All Actions for an Xcode Cloud Build 

Web Service Endpoint

# List All Actions for an Xcode Cloud Build

List all actions Xcode Cloud performed during a specific build.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciBuildRuns/{id}/actions
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Build Runs resource.

## Query Parameters

`fields[ciBuildActions]`

`[string]`

Additional fields to include for each Actions resource returned by the response.

Possible Values: `name, actionType, startedDate, finishedDate, issueCounts, executionProgress, completionStatus, isRequiredToPass, buildRun, artifacts, issues, testResults`

`limit`

`integer`

The number of Actions resources to return.

Maximum: `200`

`fields[ciBuildRuns]`

`[string]`

Possible Values: `number, createdDate, startedDate, finishedDate, sourceCommit, destinationCommit, isPullRequestBuild, issueCounts, executionProgress, completionStatus, startReason, cancelReason, builds, workflow, product, sourceBranchOrTag, destinationBranch, actions, pullRequest`

`include`

`[string]`

Value: `buildRun`

## Response Codes

` 200 ``OK`

CiBuildActionsResponse

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

The example request below lists actions Xcode Cloud performed during a specific build. Use the information provided in the response to display detailed action information on a dashboard or to read additional data; for example, test results.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciBuildRuns/074e6e3e-8343-49dd-87a3-c4274ba0faab/actions
```

```
{
    "data": [
        {
            "type": "ciBuildActions",
            "id": "457284a8-7168-4c41-982a-75d764dea585",
            "attributes": {
                "name": "archive",
                "actionType": "ARCHIVE",
                "startedDate": null,
                "finishedDate": null,
                "issueCounts": null,
                "executionProgress": "PENDING",
                "completionStatus": null,
                "isRequiredToPass": true
            },
            "relationships": {
                "buildRun": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/457284a8-7168-4c41-982a-75d764dea585/relationships/buildRun",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/457284a8-7168-4c41-982a-75d764dea585/buildRun"
                    }
                },
                "artifacts": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/457284a8-7168-4c41-982a-75d764dea585/relationships/artifacts",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/457284a8-7168-4c41-982a-75d764dea585/artifacts"
                    }
                },
                "issues": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/457284a8-7168-4c41-982a-75d764dea585/relationships/issues",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/457284a8-7168-4c41-982a-75d764dea585/issues"
                    }
                },
                "testResults": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/457284a8-7168-4c41-982a-75d764dea585/relationships/testResults",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/457284a8-7168-4c41-982a-75d764dea585/testResults"
                    }
                }
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/457284a8-7168-4c41-982a-75d764dea585"
            }
        }
    ],
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciBuildRuns/074e6e3e-8343-49dd-87a3-c4274ba0faab/actions"
    },
    "meta": {
        "paging": {
            "limit": 50
        }
    }
}
```

## See Also

### Getting Build Information

Read Xcode Cloud Build Information

Get information about a specific Xcode Cloud build.

List All Builds Xcode Cloud Created in App Store Connect

List All App Store Connect and TestFlight Builds when it performed a build.

