

- App Store Connect API
-  Read App Store Experiment Information 

Web Service Endpoint

# Read App Store Experiment Information

Get information for a specific App Store version experiment.

App Store Connect API 2.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List All Experiments for an App Store Version response.

## Query Parameters

`fields[appStoreVersionExperimentTreatments]`

`[string]`

Possible Values: `name, appIcon, appIconName, promotedDate, appStoreVersionExperiment, appStoreVersionExperimentV2, appStoreVersionExperimentTreatmentLocalizations`

`fields[appStoreVersionExperiments]`

`[string]`

Possible Values: `name, platform, trafficProportion, state, reviewRequired, startDate, endDate, app, latestControlVersion, controlVersions, appStoreVersionExperimentTreatments`

`include`

`[string]`

Possible Values: `app, latestControlVersion, controlVersions, appStoreVersionExperimentTreatments`

`limit[appStoreVersionExperimentTreatments]`

`integer`

Maximum: `50`

`limit[controlVersions]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppStoreVersionExperimentV2Response

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

## Mentioned in 

App Store Connect API 2.4 release notes

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19
```

```
{
  “data” : {
    “type” : “appStoreVersionExperiments”,
    “id” : “1a22d9a7-f574-4669-b1ca-1ba88f786c19”,
    “attributes” : {
      “name” : “PPO Test 1”,
      “platform” : “IOS”,
      “trafficProportion” : 50,
      “state” : “PREPARE_FOR_SUBMISSION”,
      “reviewRequired” : true,
      “startDate” : null,
      “endDate” : null
    },
    “relationships” : {
      “appStoreVersionExperimentTreatments” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19/relationships/appStoreVersionExperimentTreatments”,
          “related” : “https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19/appStoreVersionExperimentTreatments”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19”
  }
}
```

## See Also

### Managing App Store version experiments

List All Treatments for an App Store Experiment

Get a list of all treatments for a specific App Store version experiment.

Create an App Store Experiment

Add a new experiment to an App Store version.

Modify an App Store Experiment

Update the name, the started state, and the proportion of traffic to send to an App Store experiment.

Delete an App Store Experiment

Delete a specific App Store version experiment before it starts.

Read App Store experiment information v1

Get information for a specific App Store version experiment.

Deprecated

List all treatments for an App Store Experiment v1

Get a list of all treatments for a specific App Store version experiment.

Deprecated

Modify an App Store experiment v1

Update the name, the started state, and the proportion of traffic to send to an App Store experiment.

Deprecated

Create an App Store experiment v1

Add a new experiment to an App Store version.

Deprecated

Delete an App Store Version Experiment v1

Delete a specific App Store version experiment before it starts.

Deprecated

