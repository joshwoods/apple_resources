

- App Store Connect API
-  Read Build Action Information 

Web Service Endpoint

# Read Build Action Information

Get information about a specific action Xcode Cloud performed as part of a build.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciBuildActions/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Build Actions resource.

## Query Parameters

`fields[ciBuildActions]`

`[string]`

Additional fields to include for the Build Actions resource returned by the response.

Possible Values: `name, actionType, startedDate, finishedDate, issueCounts, executionProgress, completionStatus, isRequiredToPass, buildRun, artifacts, issues, testResults`

`include`

`[string]`

The relationship data to include in the response.

Value: `buildRun`

`fields[ciBuildRuns]`

`[string]`

Additional fields to include for the Build Actions resource returned by the response.

Possible Values: `number, createdDate, startedDate, finishedDate, sourceCommit, destinationCommit, isPullRequestBuild, issueCounts, executionProgress, completionStatus, startReason, cancelReason, builds, workflow, product, sourceBranchOrTag, destinationBranch, actions, pullRequest`

## Response Codes

` 200 ``OK`

CiBuildActionResponse

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

The example request below retrieves detailed information about an action Xcode Cloud performed. It also requests detailed information about the action’s build by including the Build Runs resource in the query. Use the information provided in the response to display information on a dashboard or to access additional information; for example, information about other actions Xcode Cloud performed during the build.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciBuildActions/6034552c-6cc0-4ac3-ad18-c3d24970882d?include=buildRun
```

```
{
    "data": {
        "type": "ciBuildActions",
        "id": "6034552c-6cc0-4ac3-ad18-c3d24970882d",
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
                "data": {
                    "type": "ciBuildRuns",
                    "id": "a2c112a3-1ed1-416d-baf8-a9f46909a16a"
                },
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/6034552c-6cc0-4ac3-ad18-c3d24970882d/relationships/buildRun",
                    "related": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/6034552c-6cc0-4ac3-ad18-c3d24970882d/buildRun"
                }
            },
            "artifacts": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/6034552c-6cc0-4ac3-ad18-c3d24970882d/relationships/artifacts",
                    "related": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/6034552c-6cc0-4ac3-ad18-c3d24970882d/artifacts"
                }
            },
            "issues": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/6034552c-6cc0-4ac3-ad18-c3d24970882d/relationships/issues",
                    "related": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/6034552c-6cc0-4ac3-ad18-c3d24970882d/issues"
                }
            },
            "testResults": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/6034552c-6cc0-4ac3-ad18-c3d24970882d/relationships/testResults",
                    "related": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/6034552c-6cc0-4ac3-ad18-c3d24970882d/testResults"
                }
            }
        },
        "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/6034552c-6cc0-4ac3-ad18-c3d24970882d"
        }
    },
    "included": [
        {
            "type": "ciBuildRuns",
            "id": "a2c112a3-1ed1-416d-baf8-a9f46909a16a",
            "attributes": {
                "number": 1,
                "createdDate": "2021-08-17T17:33:22.59Z",
                "startedDate": null,
                "finishedDate": null,
                "sourceCommit": {
                    "commitSha": "SHA",
                    "message": "Summary Message\n\nSome more details about the commit message.",
                    "author": {
                        "displayName": "Source Author",
                        "avatarUrl": "https://example.com/user/avatar/author.png"
                    },
                    "committer": {
                        "displayName": "Source Committer",
                        "avatarUrl": "https://example.com/user/avatar/author.png"
                    },
                    "webUrl": "https://example.com/commit/abc123"
                },
                "destinationCommit": {
                    "commitSha": "PR_BASE_COMMIT_SHA",
                    "message": "BASE MESSAGE",
                    "author": {
                        "displayName": "Base Author",
                        "avatarUrl": "https://example.com/user/avatar/author.png"
                    },
                    "committer": {
                        "displayName": "Base Committer",
                        "avatarUrl": "https://example.com/user/avatar/author.png"
                    },
                    "webUrl": "https://example.com/commit/xyz987"
                },
                "isPullRequestBuild": false,
                "issueCounts": null,
                "executionProgress": "PENDING",
                "completionStatus": null,
                "startReason": "MANUAL",
                "cancelReason": null
            },
            "relationships": {
                "buildRun": {},
                "builds": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciBuildRuns/a2c112a3-1ed1-416d-baf8-a9f46909a16a/relationships/builds",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciBuildRuns/a2c112a3-1ed1-416d-baf8-a9f46909a16a/builds"
                    }
                },
                "actions": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciBuildRuns/a2c112a3-1ed1-416d-baf8-a9f46909a16a/relationships/actions",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciBuildRuns/a2c112a3-1ed1-416d-baf8-a9f46909a16a/actions"
                    }
                }
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/ciBuildRuns/a2c112a3-1ed1-416d-baf8-a9f46909a16a"
            }
        }
    ],
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciBuildActions/6034552c-6cc0-4ac3-ad18-c3d24970882d?include=buildRun"
    }
}
```

## See Also

### Getting Build Actions

List All Artifacts for a Build Action

List all artifacts Xcode Cloud created when it performed an action.

Read the Xcode Cloud Build Information for a Build Action

Get Xcode Cloud build information for a given build action.

List All Issues for a Build Action

List all issues that occurred for a specific action that Xcode Cloud performed as part of a build.

List All Test Results for an Xcode Cloud Test Action

List all test results for a specific test action Xcode Cloud performed as part of a build.

