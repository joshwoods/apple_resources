

- App Store Connect API
-  Add a scheduled price change to an app 

Web Service Endpoint

# Add a scheduled price change to an app

Create a scheduled price change for an app.

App Store Connect API 2.3+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appPriceSchedules
```

## HTTP Body

AppPriceScheduleCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppPriceScheduleResponse

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

App Store Connect API 2.3 release notes

## Discussion

Warning

If you use this endpoint to add a scheduled price change to your app, you can’t use `AppPriceInlineCreate` to change your app’s price.

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/appPriceSchedules
```

```
{
  "data": {
    "type": "appPriceSchedules",
    "attributes": {},
    "relationships": {
      "app": {
        "data": {
          "type": "apps",
          "id": "6447402192"
        }
      },
      "manualPrices": {
        "data": [
          {
            "type": "appPrices",
            "id": "${newprice-0}"
          },
          {
            "type": "appPrices",
            "id": "${newprice-1}"
          },
          {
            "type": "appPrices",
            "id": "${newprice-2}"
          },
          {
            "type": "appPrices",
            "id": "${newprice-3}"
          }
        ]
      },
      "baseTerritory": {
        "data": {
          "type": "territories",
          "id": "CAN"
        }
      }
    }
  },
  "included": [
    {
      "id": "${newprice-0}",
      "relationships": {
        "appPricePoint": {
          "data": {
            "type": "appPricePoints",
            "id": "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBTEIiLCJwIjoiMTAwMTQifQ"
          }
        }
      },
      "type": "appPrices",
      "attributes": {
        "startDate": null,
        "endDate": "2023-03-11"
      }
    },
    {
      "id": "${newprice-1}",
      "relationships": {
        "appPricePoint": {
          "data": {
            "type": "appPricePoints",
            "id": "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBUkciLCJwIjoiMTAwMzQifQ"
          }
        }
      },
      "type": "appPrices",
      "attributes": {
        "startDate": null,
        "endDate": "2023-03-11"
      }
    },
    {
      "id": "${newprice-2}",
      "relationships": {
        "appPricePoint": {
          "data": {
            "type": "appPricePoints",
            "id": "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDQU4iLCJwIjoiMTAwMDcifQ"
          }
        }
      },
      "type": "appPrices",
      "attributes": {
        "startDate": null,
        "endDate": "2023-03-11"
      }
    },
    {
      "id": "${newprice-3}",
      "relationships": {
        "appPricePoint": {
          "data": {
            "type": "appPricePoints",
            "id": "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDQU4iLCJwIjoiMTAwMTAifQ"
          }
        }
      },
      "type": "appPrices",
      "attributes": {
        "startDate": "2023-03-11",
        "endDate": null
      }
    }
  ]
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

List manually chosen prices for an app

List the prices you chose for a specific app.

