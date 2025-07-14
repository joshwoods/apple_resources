

- Apple Search Ads
-  Find App Eligibility Records 

Web Service Endpoint

# Find App Eligibility Records

Fetches app eligibility records by adam ID.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/apps/{adamId}/eligibilities/find
```

## Path Parameters

`adamId`

`string`

 (Required) 

A unique App Store app identifier.

## HTTP Body

Selector

The request body that includes the selector Condition. Selector objects define what data the API returns when fetching resources.

Content-Type: application/json

## Response Codes

` 200 ``OK`

EligibilityRecordListResponse

`OK`

If the call succeeds, the API returns an EligibilityRecord in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

Content-Type: \*/\*

` 400 ``Bad Request`

ApiErrorResponse

`Bad Request`

An invalid query or missing required parameters.

Content-Type: application/json

` 401 ``Unauthorized`

ApiErrorResponse

`Unauthorized`

An unauthenticated call fails to get the requested response.

Content-Type: application/json

` 403 ``Forbidden`

ApiErrorResponse

`Forbidden`

Insufficient rights to the resource.

Content-Type: application/json

` 404 ``Not Found`

ApiErrorResponse

`Not Found`

The API can’t locate the resource.

Content-Type: application/json

` 429 `

ApiErrorResponse

The API calls exceed rate-limit thresholds. See the Rate Limits subsection of Calling the Apple Search Ads API.

Content-Type: application/json

` 500 ``Internal Server Error`

ApiErrorResponse

`Internal Server Error`

The Apple Search Ads server is temporarily down or unreachable. The request may be valid, but you need to retry it later.

Content-Type: application/json

## Mentioned in 

Apple Search Ads Campaign Management API 4

## Discussion

Use this endpoint to determine whether an app is eligible to promote in a campaign. Use a Selector Condition to search for a specific country or region, DeviceClass, AgeCriteria, or SupplySource. See the EligibilityRecord object for parameter descriptions and selector condition operators.

### Payload example: Find app eligibility records

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/apps//eligibilities/find

{
    "conditions": [
        {
            "field": "countryOrRegion",
            "operator": "IN",
            "values": ["US", "MX"]
        },
        {
            "field": "supplySource",
            "operator": "EQUALS",
            "values": ["APPSTORE_TODAY_TAB"]
        }
    ],
    "pagination": {
        "offset": 0,
        "limit": 2
    }
}
```

```
{
    "data": [
        {
            "adamId": 123456789,
            "deviceClass": "IPHONE",
            "state": "ELIGIBLE",
            "minAge": 18,
            "countryOrRegion": "US",
            "supplySource": "APPSTORE_TODAY_TAB"
        },
        {
            "adamId": 123456789,
            "deviceClass": "IPAD",
            "state": "INELIGIBLE",
            "minAge": 18,
            "countryOrRegion": "US",
            "supplySource": "APPSTORE_TODAY_TAB"
        }
    ],
    "pagination": {
        "totalResults": 4,
        "startIndex": 0,
        "itemsPerPage": 2
    }
}
```

