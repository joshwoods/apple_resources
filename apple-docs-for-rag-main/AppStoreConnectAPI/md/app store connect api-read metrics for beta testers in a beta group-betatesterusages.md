

- App Store Connect API
-  Read metrics for beta testers in a beta group 

Web Service Endpoint

# Read metrics for beta testers in a beta group

Get beta tester usage metrics for a beta group.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaGroups/{id}/metrics/betaTesterUsages
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `betaGroups` resource ID from the List Beta Groups response.

## Query Parameters

`filter[betaTesters]`

`string`

An opaque resource ID that uniquely identifies the resource. Obtain the `betaTesters` resource ID from the List Beta Testers response.

`groupBy`

`[string]`

Value: `betaTesters`

`limit`

`integer`

Maximum: `200`

`period`

`string`

Possible Values: `P7D, P30D, P90D, P365D`

## Response Codes

` 200 ``OK`

AppsBetaTesterUsagesV1MetricResponse

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
https://api.appstoreconnect.apple.com/v1/betaGroups/db51edb0-a8a4-4be9-8481-09dff260ea6e/metrics/betaTesterUsages?groupBy=betaTesters&filter%5BbetaTesters%5D=1aa1fe09-bb5c-47dd-a067-a6066db1d32
```

```
{
  “data”: [
    {
      “type”: “appsBetaTesterUsages”,
      “dataPoints”: [
        {
          “start”: “2022-10-05”,
          “end”: “2023-10-05”,
          “values”: {
            “crashCount”: 13,
            “sessionCount”: 48,
            “feedbackCount”: 21
          }
        }
      ],
      “dimensions”: {
        “betaTesters”: {
          “data”: {
            “type”: “betaTesters”,
            “id”: “1aa1fe09-bb5c-47dd-a067-a6066db1d32d”
          },
          “links”: {
            “related”: “https://api.appstoreconnect.apple.com/v1/betaTesters/1aa1fe09-bb5c-47dd-a067-a6066db1d32d”,
            “groupBy”: “https://api.appstoreconnect.apple.com/v1/betaGroups/db51edb0-a8a4-4be9-8481-09dff260ea6e/metrics/betaTesterUsages?groupBy=betaTesters”
          }
        }
      }
    }
  ],
  “links”: {
    “self”: “https://api.appstoreconnect.apple.com/v1/betaTesters/842d4014-3ecc-4f80-8531-19aa800e3a53/metrics/betaTesterUsages?period=PT8760H&filter%5Bapps%5D=6448250830”
  },
  “meta”: {
    “paging”: {
      “total”: 1,
      “limit”: 50
    }
  }
}

```

## See Also

### Getting Beta Group Information

List Beta Groups

Find and list beta groups for all apps.

Read Beta Group Information

Get a specific beta group.

Read the App Information of a Beta Group

Get the app information for a specific beta group.

Read recruitment criteria for a beta group

Get the recruitment criteria information for a specific beta group.

Read build compatibilty for a beta group

Get the build compatibilty information for a specific beta group.

