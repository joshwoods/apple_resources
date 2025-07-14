

- App Store Connect API
-  List win-back offer prices 

Web Service Endpoint

# List win-back offer prices

List all prices for specific win-back offers.

App Store Connect API 3.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/winBackOffers/{id}/prices
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `winBackOffers` resource ID from the List win-back offers response.

## Query Parameters

`fields[subscriptionPricePoints]`

`[string]`

Possible Values: `customerPrice, proceeds, proceedsYear2, territory, equalizations`

`fields[territories]`

`[string]`

Value: `currency`

`fields[winBackOfferPrices]`

`[string]`

Possible Values: `territory, subscriptionPricePoint`

`filter[territory]`

`[string]`

`include`

`[string]`

Possible Values: `territory, subscriptionPricePoint`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

WinBackOfferPricesResponse

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
https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500/prices
```

```
{
  "data": [
    {
      "type": "winBackOfferPrices",
      "id": "eyJvIjoiMTA3NzgzMjY1MDAiLCJ0IjoiQ0FOIiwicCI6IjEwMTQyIn0",
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/winBackOfferPrices/eyJvIjoiMTA3NzgzMjY1MDAiLCJ0IjoiQ0FOIiwicCI6IjEwMTQyIn0"
      }
    },
    {
      "type": "winBackOfferPrices",
      "id": "eyJvIjoiMTA3NzgzMjY1MDAiLCJ0IjoiVVNBIiwicCI6IjEwMTI3In0",
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/winBackOfferPrices/eyJvIjoiMTA3NzgzMjY1MDAiLCJ0IjoiVVNBIiwicCI6IjEwMTI3In0"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500/prices"
  },
  "meta": {
    "paging": {
      "total": 2,
      "limit": 50
    }
  }
}
```

## See Also

### Endpoints

Creating and configuring win-back offers

Configure win-back offers for your auto-renewable subscriptions with the App Store Connect API.

List win-back offers

List all win-back offers for a specific subscription.

Read win-back offer information

Read details about a specific win-back offer.

Create a win-back offer

Create a win-back offer for a specific subscription.

Modify a win-back offer

Edit details for a specific win-back offer.

Delete a win-back offer

Remove a win-back offer for a specific subscription.

