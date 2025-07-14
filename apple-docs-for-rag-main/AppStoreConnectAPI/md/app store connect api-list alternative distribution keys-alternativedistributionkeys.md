

- App Store Connect API
-  List alternative distribution keys 

Web Service Endpoint

# List alternative distribution keys

List the alternative distribution key for your account.

App Store Connect API 3.4.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys
```

## Query Parameters

`exists[app]`

`boolean`

`fields[alternativeDistributionKeys]`

`[string]`

Value: `publicKey`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

AlternativeDistributionKeysResponse

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys
```

```
{
  "data": [
    {
      "type": "alternativeDistributionKeys",
      "id": "050614c7-6d00-4db1-98e6-5869c8281f30",
      "attributes": {
        "publicKey": "-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEskEtS7l4Bl4321ZcP0V7H7rHnmnc\nHAiUWSFK/Hz4bzhd1ZyPYRwRv6zeuH+CiVmFrggScHVrBO0UUz+gRN73kQ==\n-----END PUBLIC KEY-----"
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys/050614c7-6d00-1234-98e6-5869c8281f30"
      }
    },
    {
      "type": "alternativeDistributionKeys",
      "id": "739970a0-9c7e-4fd1-be2c-f13204c728b7",
      "attributes": {
        "publicKey": "-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEZfD+k4321CZCu2tEx0SMsyhInL2G4lRBlF1ZDNnKBV7MPHFlDIQd92S2h37w46qrqVEivpSSWnFKVks+ZBeE5w==\n-----END PUBLIC KEY-----"
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys/739970a0-9c7e-2222-be2c-f13204c728b7"
      }
    },
    {
      "type": "alternativeDistributionKeys",
      "id": "ac79daa8-f11c-4c38-b244-4c7a464dbf82",
      "attributes": {
        "publicKey": "-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAE38Gko2k5454321/+bSb/rMd2BRU0\nRZoHKRMm214cqeickeWFVpOQMHXOvOuhS+i3pX7fiVGvMthanQP2KIwiZQ==\n-----END PUBLIC KEY-----"
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys/ac79daa8-f11c-ffff-b244-4c7a464dbf82"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys"
  },
  "meta": {
    "paging": {
      "total": 3,
      "limit": 50
    }
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

Read alternative distribution key information

Read the public key information for a specific alternative distribution key.

Remove an alternative distribution key

Remove an alternative distribution key from your account.

