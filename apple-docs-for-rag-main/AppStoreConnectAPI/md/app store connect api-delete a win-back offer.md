

- App Store Connect API
-  Delete a win-back offer 

Web Service Endpoint

# Delete a win-back offer

Remove a win-back offer for a specific subscription.

App Store Connect API 3.6+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/winBackOffers/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `winBackOffers` resource ID from the List win-back offers response.

## Response Codes

` 204 ``No Content`

`No Content`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

## Discussion

- Request
- Response

```
```

```
    204
```

## See Also

### Endpoints

Creating and configuring win-back offers

Configure win-back offers for your auto-renewable subscriptions with the App Store Connect API.

List win-back offers

List all win-back offers for a specific subscription.

Read win-back offer information

Read details about a specific win-back offer.

List win-back offer prices

List all prices for specific win-back offers.

Create a win-back offer

Create a win-back offer for a specific subscription.

Modify a win-back offer

Edit details for a specific win-back offer.

