

- App Store Connect API
-  List marketplace domains Deprecated

Web Service Endpoint

# List marketplace domains

List all the alternative marketplace domains for your account.

App Store Connect API 3.3–3.4.1Deprecated

Deprecated

Use List alternative distribution domains instead.

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/marketplaceDomains
```

## Query Parameters

`fields[marketplaceDomains]`

`[string]`

Possible Values: `domain, referenceName, createdDate`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

MarketplaceDomainsResponse

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
https://api.appstoreconnect.apple.com/v1/marketplaceDomains
```

```
{
  "data" : [ {
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
  }, {
    "type" : "marketplaceDomains",
    "id" : "59ee50aa-f654-46a3-b7c5-946a14c0fbbd",
    "attributes" : {
      "domain" : "apple.com",
      "referenceName" : "Apple",
      "createdDate" : "2024-01-18T23:39:24Z"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/marketplaceDomains/59ee50aa-f654-46a3-b7c5-946a14c0fbbd"
    }
  } ],
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/marketplaceDomains"
  },
  "meta" : {
    "paging" : {
      "total" : 2,
      "limit" : 50
    }
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

Read marketplace domain information

Read information for a specific alternative marketplace domain.

Deprecated

Delete a marketplace domain

Delete the alternative marketplace search domain for an app.

Deprecated

