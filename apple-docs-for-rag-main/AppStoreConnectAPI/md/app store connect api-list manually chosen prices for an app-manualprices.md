

- App Store Connect API
-  List manually chosen prices for an app 

Web Service Endpoint

# List manually chosen prices for an app

List the prices you chose for a specific app.

App Store Connect API 2.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appPriceSchedules/{id}/manualPrices
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[appPricePoints]`

`[string]`

Possible Values: `customerPrice, proceeds, app, equalizations, territory`

`fields[appPrices]`

`[string]`

Possible Values: `manual, startDate, endDate, appPricePoint, territory`

`fields[territories]`

`[string]`

Value: `currency`

`filter[endDate]`

`[string]`

`filter[startDate]`

`[string]`

`filter[territory]`

`[string]`

`include`

`[string]`

Possible Values: `appPricePoint, territory`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

AppPricesV2Response

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
https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/manualPrices?limit=200&include=appPricePoint,territory&fields%5BappPricePoints%5D=customerPrice&filter%5Bterritory%5D=USA,CAN&fields%5Bterritories%5D=currency
```

```
{
  "data" : [ {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDQU4iLCJwIjoiMTAwMDciLCJzZCI6MC4wLCJlZCI6MC4wfQ",
    "attributes" : {
      "manual" : true,
      "startDate" : null,
      "endDate" : null
    },
    "relationships" : {
      "appPricePoint" : {
        "data" : {
          "type" : "appPricePoints",
          "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDQU4iLCJwIjoiMTAwMDcifQ"
        }
      },
      "territory" : {
        "data" : {
          "type" : "territories",
          "id" : "CAN"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDQU4iLCJwIjoiMTAwMDciLCJzZCI6MC4wLCJlZCI6MC4wfQ"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJVU0EiLCJwIjoiMTAwMDciLCJzZCI6MC4wLCJlZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDB9",
    "attributes" : {
      "manual" : true,
      "startDate" : null,
      "endDate" : "2023-02-28"
    },
    "relationships" : {
      "appPricePoint" : {
        "data" : {
          "type" : "appPricePoints",
          "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJVU0EiLCJwIjoiMTAwMDcifQ"
        }
      },
      "territory" : {
        "data" : {
          "type" : "territories",
          "id" : "USA"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJVU0EiLCJwIjoiMTAwMDciLCJzZCI6MC4wLCJlZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDB9"
    }
  } ],
  "included" : [ {
    "type" : "appPricePoints",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDQU4iLCJwIjoiMTAwMDcifQ",
    "attributes" : {
      "customerPrice" : "9.99"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v3/appPricePoints/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDQU4iLCJwIjoiMTAwMDcifQ"
    }
  }, {
    "type" : "territories",
    "id" : "CAN",
    "attributes" : {
      "currency" : "CAD"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/territories/CAN"
    }
  }, {
    "type" : "appPricePoints",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJVU0EiLCJwIjoiMTAwMDcifQ",
    "attributes" : {
      "customerPrice" : "0.89"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v3/appPricePoints/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJVU0EiLCJwIjoiMTAwMDcifQ"
    }
  }, {
    "type" : "territories",
    "id" : "USA",
    "attributes" : {
      "currency" : "USD"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/territories/USA"
    }
  } ],
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/manualPrices?include=appPricePoint%2Cterritory&fields%5BappPricePoints%5D=customerPrice&filter%5Bterritory%5D=CAN%2CUSA&limit=200&fields%5Bterritories%5D=currency"
  },
  "meta" : {
    "paging" : {
      "total" : 2,
      "limit" : 200
    }
  }

```

## See Also

### Getting and managing an app’s price schedules

Read price schedule information for an app

Read price schedule details for a specific app.

Read an app's price schedule information

List the price schedule details for a specific app.

List automatically generated prices for an app

List the automatically calculated prices for an app generated from a base territory.

Read the base territory for an app's price schedule

Read the base territory and currency for a specific app.

Add a scheduled price change to an app

Create a scheduled price change for an app.

