

- Sign in with Apple REST API
-  Get a Sign in with Apple button that is left-aligned. 

Web Service Endpoint

# Get a Sign in with Apple button that is left-aligned.

Sign in with Apple REST API 1.0+

## URL

``` source
GET https://appleid.cdn-apple.com/appleid/button/left
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

`height`

`int32`

Default: `30`

Minimum: `30`

Maximum: `64`

`label-position`

`int32`

Default: `0`

Minimum: `0`

Maximum: `182`

`locale`

`string`

`logo-position`

`int32`

Default: `0`

Minimum: `0`

Maximum: `182`

`logo-size`

`string`

`scale`

`int32`

Default: `1`

Minimum: `1`

Maximum: `6`

`type`

`string`

Default: `sign-in`

`width`

`int32`

Default: `140`

Minimum: `130`

Maximum: `375`

## Response Codes

` 200 ``OK`

`binary`

`OK`

Content-Type: image/png

` 404 ``Not Found`

`Not Found`

Content-Type: application/json

