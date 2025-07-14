

- App Store Connect API
-  Read beta tester usage metrics 

Web Service Endpoint

# Read beta tester usage metrics

Get usage metrics for a specific beta tester.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaTesters/{id}/metrics/betaTesterUsages
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `betaTesters` resource ID from the List Beta Testers response.

## Query Parameters

`filter[apps]`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `apps` resource ID from the List Apps response.

`limit`

`integer`

Maximum: `200`

`period`

`string`

Possible Values: `P7D, P30D, P90D, P365D`

## Response Codes

` 200 ``OK`

BetaTesterUsagesV1MetricResponse

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
https://api.appstoreconnect.apple.com/v1/betaTesters/1aa1fe09-bb5c-47dd-a067-a6066db1d32d/metrics/betaTesterUsages?period=P90D&filter%5Bapps%5D=6447306070
```

```
{  "data": [
    {
      "type": "betaTesterUsages",
      "dataPoints": [
        {
          "start": "2023-07-07",
          "end": "2023-10-05",
          "values": {
            "crashCount": 11,
            "sessionCount": 9,
            "feedbackCount": 21
          }
        }
      ],
      "dimensions": {
        "apps": {
          "data": {
            "type": "apps",
            "id": "6447306070"
          },
          "links": {
            "related": "https://api.appstoreconnect.apple.com/v1/apps/6447306070"
          }
        }
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/betaTesters/1aa1fe09-bb5c-47dd-a067-a6066db1d32d/metrics/betaTesterUsages?period=PT2160H&filter%5Bapps%5D=6447306070"
  },
  "meta": {
    "paging": {
      "total": 1,
      "limit": 50
    }
  }
}
```

## See Also

### Beta Tester Metrics

Read beta tester metrics for an app

Get usage metrics for beta testers of a specific app.

Read metrics for beta testers in a beta group

Get beta tester usage metrics for a beta group.

