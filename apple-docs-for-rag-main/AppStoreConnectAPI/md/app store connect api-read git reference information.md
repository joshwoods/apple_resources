

- App Store Connect API
-  Read Git Reference Information 

Web Service Endpoint

# Read Git Reference Information

Get information about a specific Git reference.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/scmGitReferences/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Git References resource.

## Query Parameters

`fields[scmGitReferences]`

`[string]`

Additional fields to include for the Git References resource returned by the response.

Possible Values: `name, canonicalName, isDeleted, kind, repository`

`include`

`[string]`

The relationship data to include in the response.

Value: `repository`

## Response Codes

` 200 ``OK`

ScmGitReferenceResponse

`OK`

The request completed successfully.

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

