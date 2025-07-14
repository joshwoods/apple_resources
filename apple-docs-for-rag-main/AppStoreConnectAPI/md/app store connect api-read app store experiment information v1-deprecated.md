

- App Store Connect API
-  Read App Store experiment information v1 Deprecated

Web Service Endpoint

# Read App Store experiment information v1

Get information for a specific App Store version experiment.

App Store Connect API 1.7–2.4Deprecated

Deprecated

Use Read App Store Experiment Information instead.

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersionExperiments/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appStoreVersionExperimentTreatments]`

`[string]`

Possible Values: `name, appIcon, appIconName, promotedDate, appStoreVersionExperiment, appStoreVersionExperimentV2, appStoreVersionExperimentTreatmentLocalizations`

`fields[appStoreVersionExperiments]`

`[string]`

Possible Values: `name, trafficProportion, state, reviewRequired, startDate, endDate, appStoreVersion, appStoreVersionExperimentTreatments`

`include`

`[string]`

Possible Values: `appStoreVersion, appStoreVersionExperimentTreatments`

`limit[appStoreVersionExperimentTreatments]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppStoreVersionExperimentResponse

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

## See Also

### Managing App Store version experiments

Read App Store Experiment Information

Get information for a specific App Store version experiment.

List All Treatments for an App Store Experiment

Get a list of all treatments for a specific App Store version experiment.

Create an App Store Experiment

Add a new experiment to an App Store version.

Modify an App Store Experiment

Update the name, the started state, and the proportion of traffic to send to an App Store experiment.

Delete an App Store Experiment

Delete a specific App Store version experiment before it starts.

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

