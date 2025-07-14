

- App Store Connect API
-  List All Treatments for an App Store Experiment 

Web Service Endpoint

# List All Treatments for an App Store Experiment

Get a list of all treatments for a specific App Store version experiment.

App Store Connect API 2.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/{id}/appStoreVersionExperimentTreatments
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List All Experiments for an App Store Version response.

## Query Parameters

`fields[appStoreVersionExperimentTreatmentLocalizations]`

`[string]`

Possible Values: `locale, appStoreVersionExperimentTreatment, appScreenshotSets, appPreviewSets`

`fields[appStoreVersionExperimentTreatments]`

`[string]`

Possible Values: `name, appIcon, appIconName, promotedDate, appStoreVersionExperiment, appStoreVersionExperimentV2, appStoreVersionExperimentTreatmentLocalizations`

`fields[appStoreVersionExperiments]`

`[string]`

Possible Values: `name, trafficProportion, state, reviewRequired, startDate, endDate, appStoreVersion, appStoreVersionExperimentTreatments, platform, app, latestControlVersion, controlVersions`

`include`

`[string]`

Possible Values: `appStoreVersionExperiment, appStoreVersionExperimentV2, appStoreVersionExperimentTreatmentLocalizations`

`limit`

`integer`

Maximum: `200`

`limit[appStoreVersionExperimentTreatmentLocalizations]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppStoreVersionExperimentTreatmentsResponse

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19/appStoreVersionExperimentTreatments
```

```
{
  “data” : [ {
    “type” : “appStoreVersionExperimentTreatments”,
    “id” : “0af1be11-a7d9-4e94-aef5-f8ea12bc3be7”,
    “attributes” : {
      “name” : “Treatment Bravo”,
      “appIcon” : null,
      “appIconName” : null,
      “promotedDate” : null
    },
    “relationships” : {
      “appStoreVersionExperimentTreatmentLocalizations” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatments/0af1be11-a7d9-4e94-aef5-f8ea12bc3be7/relationships/appStoreVersionExperimentTreatmentLocalizations”,
          “related” : “https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatments/0af1be11-a7d9-4e94-aef5-f8ea12bc3be7/appStoreVersionExperimentTreatmentLocalizations”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatments/0af1be11-a7d9-4e94-aef5-f8ea12bc3be7”
    }
  }, {
    “type” : “appStoreVersionExperimentTreatments”,
    “id” : “a84d0df3-4c16-4073-adbd-90b94c742c68”,
    “attributes” : {
      “name” : “Treatment Alpha”,
      “appIcon” : null,
      “appIconName” : null,
      “promotedDate” : null
    },
    “relationships” : {
      “appStoreVersionExperimentTreatmentLocalizations” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatments/a84d0df3-4c16-4073-adbd-90b94c742c68/relationships/appStoreVersionExperimentTreatmentLocalizations”,
          “related” : “https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatments/a84d0df3-4c16-4073-adbd-90b94c742c68/appStoreVersionExperimentTreatmentLocalizations”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatments/a84d0df3-4c16-4073-adbd-90b94c742c68”
    }
  } ],
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19/appStoreVersionExperimentTreatments”
  },
  “meta” : {
    “paging” : {
      “total” : 2,
      “limit” : 50
    }
  }
}
```

## See Also

### Managing App Store version experiments

Read App Store Experiment Information

Get information for a specific App Store version experiment.

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

