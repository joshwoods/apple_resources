

- App Store Connect API
-  Read marketplace domain information Deprecated

Web Service Endpoint

# Read marketplace domain information

Read information for a specific alternative marketplace domain.

App Store Connect API 3.3–3.4.1Deprecated

Deprecated

Use Read alternative distribution domain information instead.

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/marketplaceDomains/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `marketplace domain` resource ID from the List marketplace domains response.

## Query Parameters

`fields[marketplaceDomains]`

`[string]`

Possible Values: `domain, referenceName, createdDate`

## Response Codes

` 200 ``OK`

MarketplaceDomainResponse

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
https://api.appstoreconnect.apple.com/v1/marketplaceDomains/5b74f5e8-1d7d-48a6-afd3-9441f9027292
```

```
{
  "data" : {
    "type" : "marketplaceDomains",
    "id" : "5b74f5e8-1d7d-48a6-afd3-9441f9027292",
    "attributes" : {
      "domain" : "example.com",
      "referenceName" : "exampleREF",
      "createdDate" : "2024-02-02T08:05:32Z"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/marketplaceDomains/5b74f5e8-1d7d-48a6-afd3-9441f9027292"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/marketplaceDomains/5b74f5e8-1d7d-48a6-afd3-9441f9027292"
  }
}
```

## See Also

### Managing domains

Add an alternative distribution domain

Add an alternative distribution domain to your account.

Read alternative distribution domain information

Read information for a specific alternative distribution domain.

List alternative distribution domains

List all the alternative distribution domains for your account.

Delete an alternative distribution domain

Delete the alternative distribution search domain for an app.

Add a marketplace domain

Add an alternative marketplace domain to your account.

Deprecated

List marketplace domains

List all the alternative marketplace domains for your account.

Deprecated

Delete a marketplace domain

Delete the alternative marketplace search domain for an app.

Deprecated

