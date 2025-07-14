

- App Store Connect API
-  Modify a marketplace search detail URL 

Web Service Endpoint

# Modify a marketplace search detail URL

Update the search detail URL for the alternative marketplace.

App Store Connect API 3.3+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/marketplaceSearchDetails/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `marketplace search details` resource ID from the Read the marketplace search detail URL response.

## HTTP Body

MarketplaceSearchDetailUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

MarketplaceSearchDetailResponse

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
PATCH https://api.appstoreconnect.apple.com/v1/marketplaceSearchDetails/cfcfc44f-8291-4b75-84f0-4d9a55e8b878
{
  "data": {
    "type": "marketplaceSearchDetails",
    "id": "cfcfc44f-8291-4b75-84f0-4d9a55e8b878",
    "attributes": {
      "catalogUrl": "https://example2.com/crawler-site/sitemap.xml"
    }
  }
}
```

```
{
  "data": {
    "type": "marketplaceSearchDetails",
    "id": "cfcfc44f-8291-4b75-84f0-4d9a55e8b878",
    "attributes": {
      "catalogUrl": "https://example2.com/crawler-site/sitemap.xml"
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/marketplaceSearchDetails/cfcfc44f-8291-4b75-84f0-4d9a55e8b878"
    }
  }
}
```

## See Also

### Managing search URLs

Building a searchable catalog for your marketplace app for inclusion in Spotlight

Set up and build your alternative marketplace’s searchable index.

Add a marketplace search detail URL

Add a search detail URL for the alternative marketplace.

Read the marketplace search detail URL

Get search detail URL for the alternative marketplace.

Delete a marketplace search detail URL

Delete search detail URL for the alternative marketplace.

