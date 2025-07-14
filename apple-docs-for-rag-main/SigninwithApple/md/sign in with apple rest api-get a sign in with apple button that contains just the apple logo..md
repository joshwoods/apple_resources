

- Sign in with Apple REST API
-  Get a Sign in with Apple button that contains just the Apple logo. 

Web Service Endpoint

# Get a Sign in with Apple button that contains just the Apple logo.

## URL

``` source
GET https://appleid.cdn-apple.com/appleid/button/logo
```

## Query Parameters

`border`

`boolean`

Default: `false`

`border_radius`

`int32`

Default: `15`

Minimum: `0`

Maximum: `50`

`color`

`string`

Default: `black`

`scale`

`int32`

Default: `1`

Minimum: `1`

Maximum: `6`

`size`

`int32`

Default: `30`

Minimum: `30`

Maximum: `64`

## Response Codes

` 200 ``OK`

`binary`

`OK`

Content-Type: image/png

` 404 ``Not Found`

`Not Found`

Content-Type: application/json

