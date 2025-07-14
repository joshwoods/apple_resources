

- App Store Connect API
-  Read build compatibilty for a beta group 

Web Service Endpoint

# Read build compatibilty for a beta group

Get the build compatibilty information for a specific beta group.

App Store Connect API 3.8+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaGroups/{id}/betaRecruitmentCriterionCompatibleBuildCheck
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the beta group resource ID from the List Beta Groups response.

## Query Parameters

`fields[betaRecruitmentCriterionCompatibleBuildChecks]`

`[string]`

Value: `hasCompatibleBuild`

## Response Codes

` 200 ``OK`

BetaRecruitmentCriterionCompatibleBuildCheckResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## See Also

### Getting Beta Group Information

List Beta Groups

Find and list beta groups for all apps.

Read Beta Group Information

Get a specific beta group.

Read the App Information of a Beta Group

Get the app information for a specific beta group.

Read metrics for beta testers in a beta group

Get beta tester usage metrics for a beta group.

Read recruitment criteria for a beta group

Get the recruitment criteria information for a specific beta group.

