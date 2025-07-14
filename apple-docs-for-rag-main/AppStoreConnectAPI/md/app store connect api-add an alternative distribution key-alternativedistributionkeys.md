

- App Store Connect API
-  Add an alternative distribution key 

Web Service Endpoint

# Add an alternative distribution key

Add an alternative distribution key for your alternative marketplace app or web distribution.

App Store Connect API 3.3+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys
```

## HTTP Body

AlternativeDistributionKeyCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AlternativeDistributionKeyResponse

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

## Mentioned in 

Creating and configuring keys for web distribution

Creating keys and establishing alternative marketplace connections

Configuring alternative marketplaces and alternative marketplace apps

## Discussion

You can use a single alternative distribution key for all alternative distribution apps on your account. You can optionally use an app specific alternative distribution key, by adding a relationship to a specific app in the JSON payload used with this endpoint.

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys
{
  "data": {
    "type": "alternativeDistributionKeys",
    "id": null,
    "attributes": {
      "publicKey": "-----BEGIN PUBLIC KEY-----MFkwEwYHKoZIzj0CAQYIKoZIzj0DA7021gAEFQUkD1YB67wg3e0VD/2c3N3Wf92nuQqDgFZuYG/NcYLwT3Zdw77s6//8XSI2NYv7WNgUONxMj+j65Qijq4/fhw==-----END PUBLIC KEY-----"
    }
  }
}
```

```
{
  “data” : {
    “type” : “alternativeDistributionKeys”,
    “id” : “52c5cb04-1163-65ar-36aa-a3433cd6a4f6”,
    “attributes” : {
      “publicKey” : “-----BEGIN PUBLIC KEY-----MFkwEwYHKoZIzj0CAQYIKoZIzj0DA7021gAEFQUkD1YB67wg3e0VD/2c3N3Wf92nuQqDgFZuYG/NcYLwT3Zdw77s6//8XSI2NYv7WNgUONxMj+j65Qijq4/fhw==-----END PUBLIC KEY-----”
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys/52c5cb04-1163-4a30-ad4f-a3433cd6a4f6”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/apps/6476788026/alternativeDistributionKeys”
  }
}

```

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys
{
  "data": {
    "type": "alternativeDistributionKeys",
    "id": null,
    "attributes": {
      "publicKey": "-----BEGIN PUBLIC KEY-----
MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEFQUkD1YB67wg3e0VD/2c3N3Wf92n
uQqDgFZuYG/NcYLwT3Zdw77s6//8XSI2NYv7WNgUONxMj+j65Qijq4/fhw==
-----END PUBLIC KEY-----"
    },
    "relationships": {
      "app": {
        "data": {
          "type": "apps",
          "id": "6476788026"
        }
      }
    }
  }
}
```

```
{
  "data" : {
    "type" : "alternativeDistributionKeys",
    "id" : "52c5cb04-1163-4a30-ad4f-a3433cd6a4f6",
    "attributes" : {
      "publicKey" : "-----BEGIN PUBLIC KEY-----
MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEFQUkD1YB67wg3e0VD/2c3N3Wf92n
uQqDgFZuYG/NcYLwT3Zdw77s6//8XSI2NYv7WNgUONxMj+j65Qijq4/fhw==
-----END PUBLIC KEY-----"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys/52c5cb04-1163-4a30-ad4f-a3433cd6a4f6"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/apps/6476788026/alternativeDistributionKeys"
  }
}
```

## See Also

### Creating and reading keys

Creating keys and establishing alternative marketplace connections

Manage keys you use to sign JSON web tokens and connect marketplaces with apps.

Creating and configuring keys for web distribution

Manage keys you use to sign JSON web tokens (JWTs).

List alternative distribution keys

List the alternative distribution key for your account.

Read alternative distribution key information

Read the public key information for a specific alternative distribution key.

Remove an alternative distribution key

Remove an alternative distribution key from your account.

