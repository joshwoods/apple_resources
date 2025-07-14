

- App Store Connect API
-  Add a marketplace domain Deprecated

Web Service Endpoint

# Add a marketplace domain

Add an alternative marketplace domain to your account.

App Store Connect API 3.3–3.4.1Deprecated

Deprecated

Use Add an alternative distribution domain instead.

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/marketplaceDomains
```

## HTTP Body

MarketplaceDomainCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

MarketplaceDomainResponse

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

Building a searchable catalog for your marketplace app for inclusion in Spotlight

## Discussion

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/marketplaceDomains
```

```
{
  "data" : {
    "type" : "marketplaceDomains",
    "id" : "5b74f5e8-1d7d-48a6-afd3-9441f9027292",
    "attributes" : {
      "domain" : "example.com",
      "referenceName" : "exampleREF",
      "createdDate" : "2024-02-06T07:50:59Z"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/marketplaceDomains/f6450d6a-25c7-419d-becb-4d5869b114d1"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/marketplaceDomains"
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

Read marketplace domain information

Read information for a specific alternative marketplace domain.

Deprecated

List marketplace domains

List all the alternative marketplace domains for your account.

Deprecated

Delete a marketplace domain

Delete the alternative marketplace search domain for an app.

Deprecated

