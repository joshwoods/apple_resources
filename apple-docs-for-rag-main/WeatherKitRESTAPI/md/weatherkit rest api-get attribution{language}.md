

- WeatherKit REST API
-  GET /attribution/{language} 

Web Service Endpoint

# GET /attribution/{language}

Receive attribution information.

Weather API 1.0.0+

## URL

``` source
GET https://weatherkit.apple.com/attribution/{language}
```

## Path Parameters

`language`

`string`

 (Required) 

The language tag to use for localizing responses.

## Response Codes

` 200 ``OK`

Attribution

`OK`

The request is successful. The attribution information is in the response.

Content-Type: application/json

## See Also

### Performing attribution

object Attribution

A list of image asset URLs for attribution.

