

- App Store Connect API
-  POST /v1/appStoreVersionPromotions 

Web Service Endpoint

# POST /v1/appStoreVersionPromotions

App Store Connect API 1.7+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appStoreVersionPromotions
```

## HTTP Body

AppStoreVersionPromotionCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppStoreVersionPromotionResponse

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

