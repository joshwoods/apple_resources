

- App Store Connect API
-  Add a marketplace search detail URL 

Web Service Endpoint

# Add a marketplace search detail URL

Add a search detail URL for the alternative marketplace.

App Store Connect API 3.3+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/marketplaceSearchDetails
```

## HTTP Body

MarketplaceSearchDetailCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

MarketplaceSearchDetailResponse

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

App Store Connect API 3.3 release notes

Configuring alternative marketplaces and alternative marketplace apps

## Discussion

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/marketplaceSearchDetails
{
  "data": {
    "type": "marketplaceSearchDetails",
    "attributes": {
      "catalogUrl": "https://example.com/crawler-site/sitemap.xml"
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
  “data” : {
    “type” : “marketplaceSearchDetails”,
    “id” : “cfcfc44f-8291-4b75-84f0-4d9a55e8b878”,
    “attributes” : {
      “catalogUrl” : “https://example.com/crawler-site/sitemap.xml”
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/marketplaceSearchDetails/cfcfc44f-8291-4b75-84f0-4d9a55e8b878”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/apps/6476788026/marketplaceSearchDetail”
  }
}

```

## See Also

### Managing search URLs

Building a searchable catalog for your marketplace app for inclusion in Spotlight

Set up and build your alternative marketplace’s searchable index.

Read the marketplace search detail URL

Get search detail URL for the alternative marketplace.

Modify a marketplace search detail URL

Update the search detail URL for the alternative marketplace.

Delete a marketplace search detail URL

Delete search detail URL for the alternative marketplace.

