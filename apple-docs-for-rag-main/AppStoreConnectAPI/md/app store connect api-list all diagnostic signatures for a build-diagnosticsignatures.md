

- App Store Connect API
-  List All Diagnostic Signatures for a Build 

Web Service Endpoint

# List All Diagnostic Signatures for a Build

List the aggregate backtrace signatures captured for a specific build.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/builds/{id}/diagnosticSignatures
```

## Path Parameters

`id`

`string`

 (Required) 

The resource ID that uniquely identifies the build to return metrics data for. Obtain the build resource ID from the List Builds response.

## Query Parameters

`fields[diagnosticSignatures]`

`[string]`

Fields to return for diagnostic signatures.

Possible Values: `diagnosticType, signature, weight, insight, logs`

`filter[diagnosticType]`

`[string]`

The diagnostic types by which to filter.

Possible Values: `DISK_WRITES, HANGS, LAUNCHES`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

DiagnosticSignaturesResponse

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

## Mentioned in 

App Store Connect API 3.5 release notes

App Store Connect API 2.0 release notes

## Discussion

The example below requests the top two weighted disk write diagnostic signatures. The example response returns two signatures that are responsible for 85% and 7% of disk writes.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/builds/1a254ec1-8e3d-48e7-bbd6-6b9a30072b29/diagnosticSignatures?filter[diagnosticType]=DISK_WRITES&limit=2
```

```
{
  "data": [
    {
      "type": "diagnosticSignatures",
      "id": "35fd8da9ea3dd8d2a64cb3d458fa59b2b41e66115f7ca5fa34df25a9419c5216dd",
      "attributes": {
        "diagnosticType": "DISK_WRITES",
        "signature": "ExampleApp: -[DatabaseConnection executeSQL:enumerateRowsWithBlock:] + 23",
        "weight": 0.85
      },
      "relationships": {
        "logs": {
          "links": {
            "related": "https://api.appstoreconnect.apple.com/v1/diagnosticSignatures/35fd8da9ea3dd8d2a64cb3d458fa59b2b41e66115f7ca5fa34df25a9419c5216dd/logs"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/diagnosticSignatures/35fd8da9ea3dd8d2a64cb3d458fa59b2b41e66115f7ca5fa34df25a9419c5216dd"
      }
    },
    {
      "type": "diagnosticSignatures",
      "id": "351c486f96912d7520ef0ceea8efe19aca98f41e3b111a77e64f6923d6eba0e2c7",
      "attributes": {
        "diagnosticType": "DISK_WRITES",
        "signature": "ExampleApp: -[TemporaryFile appendData:] + 100",
        "weight": 0.07
      },
      "relationships": {
        "logs": {
          "links": {
            "related": "https://api.appstoreconnect.apple.com/v1/diagnosticSignatures/351c486f96912d7520ef0ceea8efe19aca98f41e3b111a77e64f6923d6eba0e2c7/logs"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/diagnosticSignatures/351c486f96912d7520ef0ceea8efe19aca98f41e3b111a77e64f6923d6eba0e2c7"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/builds/1a254ec1-8e3d-48e7-bbd6-6b9a30072b29/diagnosticSignatures?limit=3&filter%5BdiagnosticType%5D=DISK_WRITES",
    "next": "https://api.appstoreconnect.apple.com/v1/builds/1a254ec1-8e3d-48e7-bbd6-6b9a30072b29/diagnosticSignatures?cursor=Aw.AOYOFlQ&limit=3&filter%5BdiagnosticType%5D=DISK_WRITES"
  },
  "meta": {
    "paging": {
      "total": 4,
      "limit": 2
    }
  }
}
```

## See Also

### Getting Metrics and Diagnostic Logs

Retrieve Power and Performance Metrics and Log Insights

Use the App Store Connect API to collect and parse diagnostic logs and metrics for your apps.

Get Power and Performance Metrics for an App

Get the performance and power metrics data for the most recent version of an app.

Get Power and Performance Metrics for a Build

Get the performance and power metrics data for a specific build.

Download Logs for a Diagnostic Signature

Get the anonymized backtrace logs associated with a specific diagnostic signature.

