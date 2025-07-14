

- App Store Connect API
-  List automatically generated prices for an app 

Web Service Endpoint

# List automatically generated prices for an app

List the automatically calculated prices for an app generated from a base territory.

App Store Connect API 2.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appPriceSchedules/{id}/automaticPrices
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
https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/automaticPrices
```

```
{
  "data" : [ {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBRkciLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBRkciLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBR08iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBR08iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBSUEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBSUEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBUkUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBUkUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBUk0iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBUk0iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBVEciLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBVEciLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBVVMiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBVVMiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBVVQiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBVVQiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBWkUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJBWkUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCRUwiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCRUwiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCRU4iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCRU4iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCRkEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCRkEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCR1IiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCR1IiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCSFIiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCSFIiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCSFMiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCSFMiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCSUgiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCSUgiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCTFIiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCTFIiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCTFoiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCTFoiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCTVUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCTVUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCT0wiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCT0wiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCUkEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCUkEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCUkIiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCUkIiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCUk4iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCUk4iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCVE4iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCVE4iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCV0EiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJCV0EiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDSEUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDSEUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDSEwiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDSEwiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDSE4iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDSE4iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDSVYiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDSVYiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDTVIiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDTVIiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDT0QiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDT0QiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDT0ciLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDT0ciLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDT0wiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDT0wiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDUFYiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDUFYiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDUkkiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDUkkiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDWU0iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDWU0iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDWVAiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDWVAiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDWkUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJDWkUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJERVUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJERVUiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJETUEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJETUEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJETksiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJETksiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJET00iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJET00iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJEWkEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJEWkEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJFQ1UiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJFQ1UiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJFR1kiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJFR1kiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJFU1AiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJFU1AiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJFU1QiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJFU1QiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJGSU4iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJGSU4iLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJGSkkiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJGSkkiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  }, {
    "type" : "appPrices",
    "id" : "eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJGUkEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9",
    "attributes" : {
      "manual" : false,
      "startDate" : "2023-02-28",
      "endDate" : null
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appPrices/eyJzIjoiNjQ0NzQwMjE5MiIsInQiOiJGUkEiLCJwIjoiMTAwMDciLCJzZCI6MTY3NzU3MTIwMC4wMDAwMDAwMDAsImVkIjowLjB9"
    }
  } ],
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/automaticPrices",
    "next" : "https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/automaticPrices?cursor=Mg.AKwzESA"
  },
  "meta" : {
    "paging" : {
      "total" : 172,
      "limit" : 50
    }
  }
}
```

## See Also

### Getting and managing an app’s price schedules

Read price schedule information for an app

Read price schedule details for a specific app.

Read an app's price schedule information

List the price schedule details for a specific app.

Read the base territory for an app's price schedule

Read the base territory and currency for a specific app.

List manually chosen prices for an app

List the prices you chose for a specific app.

Add a scheduled price change to an app

Create a scheduled price change for an app.

