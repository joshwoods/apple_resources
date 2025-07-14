

- App Store Connect API
-  Get Power and Performance Metrics for a Build 

Web Service Endpoint

# Get Power and Performance Metrics for a Build

Get the performance and power metrics data for a specific build.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/builds/{id}/perfPowerMetrics
```

## Path Parameters

`id`

`string`

 (Required) 

The resource ID that uniquely identifies the build to return metrics data for. Obtain the build resource ID from the List Builds response.

## Query Parameters

`filter[deviceType]`

`[string]`

Device types by which to filter. Use `all_iphones` for all iPhone models. Use `all_ipads` for all iPad models.

`filter[metricType]`

`[string]`

Types of metrics by which to filter. For more information about metric types, see MetricCategory.

Possible Values: `DISK, HANG, BATTERY, LAUNCH, MEMORY, ANIMATION, TERMINATION`

`filter[platform]`

`[string]`

Platforms by which to filter.

Value: `IOS`

## Response Codes

` 200 ``OK`

xcodeMetrics

`OK`

Content-Type: application/vnd.apple.xcode-metrics+json

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

## Mentioned in 

App Store Connect API 1.4 release notes

## Discussion

The example below requests iOS animation metrics on all iPads for a specific build. To get the metrics for all of the most-recent app versions instead, use the Get Power and Performance Metrics for an App endpoint.

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/builds/43d3a970-273c-4bc9-88ee-aa5c05610ac1/perfPowerMetrics?filter[deviceType]=all_ipads&filter[metricType]=ANIMATION&filter[platform]=iOS
```

```
{
  "productData": [
    {
      "platform": "iOS",
      "metricCategories": [
        {
          "identifier": "ANIMATION",
          "metrics": [
            {
              "identifier": "scrollHitchRate",
              "unit": {
                "identifier": "scrollHitchRate",
                "displayName": "%"
              },
              "datasets": [
                {
                  "filterCriteria": {
                    "percentile": "percentile.fifty",
                    "device": "all_ipads",
                    "deviceMarketingName": "All iPads"
                  },
                  "points": [
                    {
                      "version": "10.0",
                      "value": 6.5,
                      "goal": "fair"
                    }
                  ]
                },
                {
                  "filterCriteria": {
                    "percentile": "percentile.ninety",
                    "device": "all_ipads",
                    "deviceMarketingName": "All iPads"
                  },
                  "points": [
                    {
                      "version": "10.0",
                      "value": 29.7,
                      "goal": "poor"
                    }
                  ]
                }
              ],
              "goalKeys": [
                {
                  "goalKey": "poor",
                  "lowerBound": 10
                },
                {
                  "upperBound": 10,
                  "goalKey": "fair",
                  "lowerBound": 5
                },
                {
                  "upperBound": 5,
                  "goalKey": "good",
                  "lowerBound": 0
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "version": "1.0.0"
}
```

## See Also

### Getting Metrics and Diagnostic Logs

Retrieve Power and Performance Metrics and Log Insights

Use the App Store Connect API to collect and parse diagnostic logs and metrics for your apps.

Get Power and Performance Metrics for an App

Get the performance and power metrics data for the most recent version of an app.

List All Diagnostic Signatures for a Build

List the aggregate backtrace signatures captured for a specific build.

Download Logs for a Diagnostic Signature

Get the anonymized backtrace logs associated with a specific diagnostic signature.

