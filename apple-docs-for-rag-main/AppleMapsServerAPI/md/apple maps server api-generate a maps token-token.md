

- Apple Maps Server API
-  Generate a Maps token 

Web Service Endpoint

# Generate a Maps token

Returns a JWT maps access token that you use to call the service API.

Apple Maps Server API 1.2+

## URL

``` source
GET https://maps-api.apple.com/v1/token
```

## Response Codes

` 200 ``OK`

TokenResponse

`OK`

A response that indicates the authorization request is successful. The dictionary that accompanies the response contains a maps access token and an integer that indicates the time in seconds until the token expires.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

An error response that indicates the maps token is missing or invalid. The dictionary that accompanies the error may contain additional details about the error.

Content-Type: application/json

` 429 `

ErrorResponse

An ErrorResponse object that indicates the call exceeds the daily service call quota for the authorization token presented. The app should try again later. If your app requires a larger daily quota, submit a quota increase request form.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorResponse

`Internal Server Error`

An error that indicates the server can’t complete the request. The dictionary that accompanies the error may contain additional details about the error.

Content-Type: application/json

## Mentioned in 

Creating and using tokens with Maps Server API

## Discussion

### Example

- Request
- Response

```
curl -si -H "Authorization: Bearer " "https://maps-api.apple.com/v1/token"
```

```
{
  "accessToken": "",
  "expiresInSeconds": 1800
}
```

## See Also

### Essentials

Creating and using tokens with Maps Server API

Sign JSON Web Tokens to use Maps Server API and debug common signing errors.

Creating a Maps identifier and a private key

Create a Maps identifier and a private key before generating tokens for MapKit JS.

Debugging an Invalid token

Inspect the JavaScript console logs, the token, and events to determine why a token is invalid.

Common objects

Understand the common JSON objects that API responses contain.

Integrating the Apple Maps Server API into Java server applications

Streamline your app’s API by moving georelated searches from inside your app to your server.

