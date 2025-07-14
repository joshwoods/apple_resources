

- App Store Connect API
-  Modify a Beta App Review Detail 

Web Service Endpoint

# Modify a Beta App Review Detail

Update the details for a specific app’s beta app review.

App Store Connect API 1.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/betaAppReviewDetails/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## HTTP Body

BetaAppReviewDetailUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

BetaAppReviewDetailResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Overview

Important

First name, last name, phone, email cannot be cleared for the primary locale once set.

