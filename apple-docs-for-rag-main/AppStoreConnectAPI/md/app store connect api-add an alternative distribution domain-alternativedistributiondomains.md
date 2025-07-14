

- App Store Connect API
-  Add an alternative distribution domain 

Web Service Endpoint

# Add an alternative distribution domain

Add an alternative distribution domain to your account.

App Store Connect API 3.4.1+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/alternativeDistributionDomains
```

## HTTP Body

AlternativeDistributionDomainCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AlternativeDistributionDomainResponse

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

Configuring apps for web distribution

Configuring alternative marketplaces and alternative marketplace apps

Creating and configuring keys for web distribution

## Discussion

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/alternativeDistributionDomains
```

```
{
  “data” : {
    “type” : “alternativeDistributionDomains”,
    “id” : “5b74f5e8-1d7d-48a6-afd3-9441f9027292”,
    “attributes” : {
      “domain” : “example.com”,
      “referenceName” : “exampleREF”,
      “createdDate” : “2024-03-24T07:50:59Z”
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/alternativeDistributionDomains/f6450d6a-25c7-419d-becb-4d5869b114d1”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/alternativeDistributionDomains”
  }
}
```

## See Also

### Managing domains

Read alternative distribution domain information

Read information for a specific alternative distribution domain.

List alternative distribution domains

List all the alternative distribution domains for your account.

Delete an alternative distribution domain

Delete the alternative distribution search domain for an app.

Add a marketplace domain

Add an alternative marketplace domain to your account.

Deprecated

Read marketplace domain information

Read information for a specific alternative marketplace domain.

Deprecated

List marketplace domains

List all the alternative marketplace domains for your account.

Deprecated

Delete a marketplace domain

Delete the alternative marketplace search domain for an app.

Deprecated

