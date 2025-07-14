

- App Store Connect API
-  List All Beta Groups for an App 

Web Service Endpoint

# List All Beta Groups for an App

Get a list of beta groups associated with a specific app.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/betaGroups
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[betaGroups]`

`[string]`

Fields to return for included related types.

Possible Values: `name, createdDate, isInternalGroup, hasAccessToAllBuilds, publicLinkEnabled, publicLinkId, publicLinkLimitEnabled, publicLinkLimit, publicLink, feedbackEnabled, iosBuildsAvailableForAppleSiliconMac, iosBuildsAvailableForAppleVision, app, builds, betaTesters, betaRecruitmentCriteria, betaRecruitmentCriterionCompatibleBuildCheck`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

BetaGroupsWithoutIncludesResponse

`OK`

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

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/6446998023/betaGroups
```

```
{
    “data”: [
        {
            “type”: “betaGroups”,
            “id”: “26b3c3c4-aeb1-4d24-be6a-80c554f671a2”,
            “attributes”: {
                “name”: “Internal Test Group”,
                “createdDate”: “2022-09-07T18:25:13.582Z”,
                “isInternalGroup”: true,
                “hasAccessToAllBuilds”: true,
                “publicLinkEnabled”: null,
                “publicLinkId”: null,
                “publicLinkLimitEnabled”: null,
                “publicLinkLimit”: null,
                “publicLink”: null,
                “feedbackEnabled”: true,
                “iosBuildsAvailableForAppleSiliconMac”: true
            },

```

## See Also

### Getting beta tester information for TestFlight

Remove Specified Beta Testers from All Groups and Builds of an App

Remove one or more beta testers’ access to test any builds of a specific app.

