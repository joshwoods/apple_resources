

- App Store Connect API
-  List All Artifacts for a Build Action 

Web Service Endpoint

# List All Artifacts for a Build Action

List all artifacts Xcode Cloud created when it performed an action.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciBuildActions/{id}/artifacts
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Build Actions resource.

## Query Parameters

`fields[ciArtifacts]`

`[string]`

Additional fields to include for each Artifacts resource returned by the response.

Possible Values: `fileType, fileName, fileSize, downloadUrl`

`limit`

`integer`

The number of Artifacts resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

CiArtifactsResponse

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

### Getting Build Actions

Read Build Action Information

Get information about a specific action Xcode Cloud performed as part of a build.

Read the Xcode Cloud Build Information for a Build Action

Get Xcode Cloud build information for a given build action.

List All Issues for a Build Action

List all issues that occurred for a specific action that Xcode Cloud performed as part of a build.

List All Test Results for an Xcode Cloud Test Action

List all test results for a specific test action Xcode Cloud performed as part of a build.

