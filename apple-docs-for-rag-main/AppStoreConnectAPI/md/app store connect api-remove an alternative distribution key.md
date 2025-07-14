

- App Store Connect API
-  Remove an alternative distribution key 

Web Service Endpoint

# Remove an alternative distribution key

Remove an alternative distribution key from your account.

App Store Connect API 3.3+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `alternativeDistributionKey` resource ID from the Read an app’s alternative distribution key response.

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

### Example Request and Response

- Request
- Response

```
DELETE https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys/52c5cb04-1163-4a30-ad4f-a3433cd6a4f6
```

```
204
```

## See Also

### Creating and reading keys

Creating keys and establishing alternative marketplace connections

Manage keys you use to sign JSON web tokens and connect marketplaces with apps.

Creating and configuring keys for web distribution

Manage keys you use to sign JSON web tokens (JWTs).

Add an alternative distribution key

Add an alternative distribution key for your alternative marketplace app or web distribution.

List alternative distribution keys

List the alternative distribution key for your account.

Read alternative distribution key information

Read the public key information for a specific alternative distribution key.

