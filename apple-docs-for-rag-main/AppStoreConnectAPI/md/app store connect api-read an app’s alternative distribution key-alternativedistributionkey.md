

- App Store Connect API
-  Read an app’s alternative distribution key 

Web Service Endpoint

# Read an app’s alternative distribution key

Get the alternative distribution keys for a specific app.

App Store Connect API 3.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/alternativeDistributionKey
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `apps` ID from the List Apps response.

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

## Mentioned in 

App Store Connect API 3.7 release notes

Creating keys and establishing alternative marketplace connections

Creating and configuring keys for web distribution

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/6473805491/alternativeDistributionKey
```

```
{
  “data” : {
    “type” : “alternativeDistributionKeys”,
    “id” : “52c5cb04-1163-4a30-ad4f-a3433cd6a4f6”,
    “attributes” : {
      “publicKey” : “-----BEGIN PUBLIC KEY-----\nMFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAE7rsxeCw+hrwRgStk0J2vYmnGQZha\ngSt0fm511aTjpDVsaIy9z7jmUKjJ1jgb8P5UKmQfmw0ovD+fNTSefjrw5A==\n-----END PUBLIC KEY-----\n”
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys/52c5cb04-1163-4a30-ad4f-a3433cd6a4f6”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/apps/6473805491/alternativeDistributionKey”
  }
}
```

## See Also

### Getting alternative distribution information

Read the marketplace search detail URL

Get search detail URL for the alternative marketplace.

