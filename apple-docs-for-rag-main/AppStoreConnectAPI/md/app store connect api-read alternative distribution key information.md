

- App Store Connect API
-  Read alternative distribution key information 

Web Service Endpoint

# Read alternative distribution key information

Read the public key information for a specific alternative distribution key.

App Store Connect API 3.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `alternative Distribution Key` resource ID from the Read an app’s alternative distribution key response.

## Query Parameters

`fields[alternativeDistributionKeys]`

`[string]`

Value: `publicKey`

## Response Codes

` 200 ``OK`

AlternativeDistributionKeyResponse

`OK`

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/distributionKeys/52c5cb04-1163-4a30-ad4f-a3433cd6a4f6
```

```
{
  "data" : {
    "type" : "distributionKeys",
    "id" : "52c5cb04-1163-4a30-ad4f-a3433cd6a4f6",
    "attributes" : {
      "publicKey" : "-----BEGIN PUBLIC KEY-----
MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEFQUkD1YB67wg3e0VD/2c3N3Wf92n
uQqDgFZuYG/NcYLwT3Zdw77s6//8XSI2NYv7WNgUONxMj+j65Qijq4/fhw==
-----END PUBLIC KEY-----"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/distributionKeys/52c5cb04-1163-4a30-ad4f-a3433cd6a4f6"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/distributionKeys/52c5cb04-1163-4a30-ad4f-a3433cd6a4f6"
  }
}
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

Remove an alternative distribution key

Remove an alternative distribution key from your account.

