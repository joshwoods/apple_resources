

- Apple Maps Server API
-  Search for directions and estimated travel time between locations 

Web Service Endpoint

# Search for directions and estimated travel time between locations

Find directions by specific criteria.

Apple Maps Server API 1.2+

## URL

``` source
GET https://maps-api.apple.com/v1/directions
```

## Query Parameters

`origin`

`string`

 (Required) 

The starting location as an address, or coordinates you specify as latitude, longitude. For example, `origin=37.7857,-122.4011`

`destination`

`string`

 (Required) 

The destination as an address, or coordinates you specify as latitude, longitude. For example, `destination=San Francisco City Hall, CA`

`arrivalDate`

`string`

The date and time to arrive at the destination in ISO 8601 format in UTC time. For example, `2023-04-15T16:42:00Z`.

You can specify only `arrivalDate` or `departureDate`. If you don’t specify either option, the `departureDate` defaults to *now*, which the server interprets as the current time.

`avoid`

`[`DirectionsAvoid`]`

A comma-separated list of the features to avoid when calculating direction routes. For example, `avoid=Tolls`.

See DirectionsAvoid for a complete list of possible values.

`departureDate`

`string`

The date and time to depart from the origin in ISO 8601 format in UTC time. For example, `2023-04-15T16:42:00Z`.

You can only specify `arrivalDate` or `departureDate`. If you don’t specify either option, the `departureDate` defaults to *now*, which the server interprets as the current time.

`lang`

Lang

The language the server uses when returning the response, specified using a BCP 47 language code. For example, for English, use `lang=en-US`.

Default: `en-US`

`requestsAlternateRoutes`

`boolean`

When you set this to `true`, the server returns additional routes, when available. For example, `requestsAlternateRoutes=true.`

Default: `false`

`searchLocation`

SearchLocation

A `searchLocation` the app defines as a hint for the query input for `origin` or `destination`. Specify the location as a comma-separated string that contains the latitude and longitude. For example, `37.7857,-122.4011`.

If you don’t provide a `searchLocation`, the server uses `userLocation` and searchLocation as fallback hints.

`searchRegion`

SearchRegion

A region the app defines as a hint for the query input for `origin` or `destination`. Specify the region as a comma-separated string that describes the region in the form of a north-latitude, east-longitude, south-latitude, west-longitude string. For example, 38,-122.1,37.5,-122.5.

If you don’t provide a `searchLocation`, the server uses `userLocation` and `searchRegion` as fallback hints.

`transportType`

`string`

The mode of transportation the server returns directions for.

Default: `Automobile`

Possible Values: `Automobile, Walking`

`userLocation`

UserLocation

The location of the user, specified as a comma-separated string that contains the latitude and longitude. For example, `userLocation=37.78,-122.42`.

If you don’t provide a `searchLocation`, the server uses `userLocation` and `searchRegion` as fallback hints.

## Response Codes

` 200 ``OK`

DirectionsResponse

`OK`

Returns a DirectionsResponse result that describes the steps and routes from the origin to the destination.

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An ErrorResponse object that contains an error message and an array of strings that contain additional details about the error.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

An ErrorResponse object that contains an error message that indicates the Maps access token is missing or invalid, and an array of strings that contains additional details about the error.

Content-Type: application/json

` 429 `

ErrorResponse

An ErrorResponse object that indicates the call exceeds the daily service call quota for the authorization token. The app can try again later. If your app requires a larger daily quota, submit a quota increase request form.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorResponse

`Internal Server Error`

An ErrorResponse object that contains a server error message and an array of strings that describe additional details about the error.

Content-Type: application/json

## Discussion

### Example

- Request
- Response

```
curl -si -H "Authorization: Bearer " \
"https://maps-api.apple.com/v1/directions?origin=37.7857,-122.4011&destination=San Francisco City Hall, CA"
```

```
```

## See Also

### Directions

Determine estimated arrival times and distances to one or more destinations

Returns the estimated time of arrival (ETA) and distance between starting and ending locations.

