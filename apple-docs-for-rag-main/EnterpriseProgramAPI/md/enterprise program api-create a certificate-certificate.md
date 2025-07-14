

- Enterprise Program API
-  Create a Certificate 

Web Service Endpoint

# Create a Certificate

Create a new certificate using a certificate signing request.

## URL

``` source
POST https://api.enterprise.developer.apple.com/v1/certificates
```

## HTTP Body

CertificateCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

CertificateResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Overview

- HTTPBody

