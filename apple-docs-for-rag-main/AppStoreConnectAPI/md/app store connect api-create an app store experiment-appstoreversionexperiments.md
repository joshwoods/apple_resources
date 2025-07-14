

- App Store Connect API
-  Create an App Store Experiment 

Web Service Endpoint

# Create an App Store Experiment

Add a new experiment to an App Store version.

App Store Connect API 2.4+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments
```

## HTTP Body

AppStoreVersionExperimentV2CreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppStoreVersionExperimentV2Response

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Mentioned in 

App Store Connect API 2.4 release notes

## Discussion

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments -d
‘{
  “data”: {
    “type”: “appStoreVersionExperiments”,
    “attributes”: {
      “platform”: “IOS”,
      “name”: “PPO Test 1”,
      “trafficProportion”: 66
    },
    “relationships”: {
      “app”: {
        “data”: {
          “type”: “apps”,
          “id”: “1452013590”
        }
      }
    }
  }
}’

```

```
{
  "data": {
    "type": "appStoreVersionExperiments",
    "id": "1a22d9a7-f574-4669-b1ca-1ba88f786c19",
    "attributes": {
      "name": "PPO Test 1",
      "platform": "IOS",
      "trafficProportion": 66,
      "state": "PREPARE_FOR_SUBMISSION",
      "reviewRequired": false,
      "startDate": null,
      "endDate": null
    },
    "relationships": {
      "appStoreVersionExperimentTreatments": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19/relationships/appStoreVersionExperimentTreatments",
          "related": "https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19/appStoreVersionExperimentTreatments"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments"
  }
}

```

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments -d
'{
  "data": {
    "type": "appStoreVersionExperiments",
    "attributes": {
      "platform": "IOS",
      "name": "PPO Test 1",
      "trafficProportion": 66
    },
    "relationships": {
      "app": {
        "data": {
          "type": "apps",
          "id": "1452013590"
        }
      }
    }
  }
}'
```

```
{
  "errors" : [ {
    "id" : "b47f2d6f-681f-479c-b2ff-42fd020cc9ad",
    "status" : "409",
    "code" : "STATE_ERROR",
    "title" : "The request cannot be fulfilled because of the state of another resource.",
    "detail" : "Cannot create new experiment because another experiment is in draft state"
  } ]
}
```

## See Also

### Managing App Store version experiments

Read App Store Experiment Information

Get information for a specific App Store version experiment.

List All Treatments for an App Store Experiment

Get a list of all treatments for a specific App Store version experiment.

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

