

- App Store Connect API
-  List All Xcode Cloud Builds for a Workflow 

Web Service Endpoint

# List All Xcode Cloud Builds for a Workflow

List all builds Xcode Cloud performed for a specific workflow.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciWorkflows/{id}/buildRuns
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Workflows resource.

## Query Parameters

`fields[builds]`

`[string]`

Additional fields to include for each Build Runs resource returned by the response.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`fields[ciBuildRuns]`

`[string]`

Additional fields to include for each Build Runs resource returned by the response.

Possible Values: `number, createdDate, startedDate, finishedDate, sourceCommit, destinationCommit, isPullRequestBuild, issueCounts, executionProgress, completionStatus, startReason, cancelReason, builds, workflow, product, sourceBranchOrTag, destinationBranch, actions, pullRequest`

`filter[builds]`

`[string]`

Filter the returned build runs using the ID of the related Builds resource.

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `builds, workflow, product, sourceBranchOrTag, destinationBranch, pullRequest`

`limit`

`integer`

The number of Build Runs resources to return.

Maximum: `200`

`limit[builds]`

`integer`

The number of included Build Runs resources to return if the builds relationship is included.

Maximum: `50`

`fields[scmGitReferences]`

`[string]`

Possible Values: `name, canonicalName, isDeleted, kind, repository`

`fields[ciWorkflows]`

`[string]`

Possible Values: `name, description, branchStartCondition, tagStartCondition, pullRequestStartCondition, scheduledStartCondition, manualBranchStartCondition, manualTagStartCondition, manualPullRequestStartCondition, actions, isEnabled, isLockedForEditing, clean, containerFilePath, lastModifiedDate, product, repository, xcodeVersion, macOsVersion, buildRuns`

`fields[scmPullRequests]`

`[string]`

Possible Values: `title, number, webUrl, sourceRepositoryOwner, sourceRepositoryName, sourceBranchName, destinationRepositoryOwner, destinationRepositoryName, destinationBranchName, isClosed, isCrossRepository, repository`

`fields[ciProducts]`

`[string]`

Possible Values: `name, createdDate, productType, app, bundleId, workflows, primaryRepositories, additionalRepositories, buildRuns`

`sort`

`[string]`

Possible Values: `number, -number`

## Response Codes

` 200 ``OK`

CiBuildRunsResponse

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

## See Also

### Getting Xcode Cloud Workflows

Read Xcode Cloud Workflow Information

Get information about a specific Xcode Cloud workflow.

Read the Repository Information for an Xcode Cloud Workflow

Get information about the Git repository of a specific Xcode Cloud workflow.

