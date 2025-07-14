

- Device Management
-  Get Metadata for a Catalog Book 

Web Service Endpoint

# Get Metadata for a Catalog Book

Fetch metadata for a book from the catalog by using its identifier.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://api.ent.apple.com/v1/catalog/{storefront}/books/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the catalog book.

`storefront`

`string`

 (Required) 

An iTunes Store territory that you specify with an ISO 3166 alpha-2 country code. The possible values are the `id` attributes of `Storefrontobjects`.

## Query Parameters

`additionalPlatforms`

`[string]`

Additional platforms the app supports that you want to get metadata for.

Possible Values: `appletv, ipad, iphone, mac, realityDevice, web`

`include`

`[string]`

A list of relationship names to include for resources in the response.

Classifier (optional): A resource type to apply the parameter to, `apps` or `books`.

`l`

`string`

The localization to use, which you specify with a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object that `storefront` specifies. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`platform`

`string`

 (Required) 

The platform the user-facing app is running on. You use this to get metadata for the specified platform.

Possible Values: `appletv, ipad, iphone, mac, realityDevice, web`

`relate`

`[string]`

A list of relationship names to relate for resources in the response.

Classifier (optional): A resource type to apply the parameter to, `apps` or `books`.

## Response Codes

` 200 ``OK`

BooksResponse

`OK`

The request was successful.

Content-Type: application/json

` 401 ``Unauthorized`

UnauthorizedResponse

`Unauthorized`

A response indicating an incorrect `Authorization` header.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorsResponse

`Internal Server Error`

A response indicating an error occurred on the server.

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
/book_id_123?platform=iphone
```

```
{
  "data":[
    {
        "id": "book_id_123",
        "type": "books",
        "href": "/v1/catalog/us/books/book_id_123?l=en-US",
        "attributes": {
          "offers": [
            {
              "buyParams": "productType=PUB&price=13990&salableAdamId=book_id_123&pricingParameters=STDQ&pg=default&marketType=ENT",
              "type": "buy",
              "priceFormatted": "$13.99",
              "price": 13.99,
              "currencyCode": "USD",
              "assets": [
                {
                  "flavor": "publication",
                  "size": 98316906
                }
              ]
            }
          ],
          "genreNames": [
            "Art & Architecture",
            "Books",
            "Arts & Entertainment",
            "Health, Mind & Body",
            "Self-Improvement"
          ],
          "isbn": "123456789",
          "name": "A Very Famous Book",
          "artistName": "FamousAuthor",
          "artwork": {
            "width": 2213,
            "height": 2400,
            "url": "IMAGE_URL",
            "bgColor": "b7c2c4",
            "textColor1": "0e0c11",
            "textColor2": "301f1b",
            "textColor3": "303035",
            "textColor4": "4b403d"
          },
          "url": "https://books.apple.com/us/book/foo-bar/id123456",
          "userRating": {
            "value": 0,
            "ratingCount": 0
          }
        },
        "relationships": {
          "genres": {
            "href": "/v1/catalog/us/books/book_id_123/genres?l=en-US",
            "data": [
              {
                "id": "10002",
                "type": "genres",
                "href": "/v1/catalog/us/genres/10002?l=en-US",
                "attributes": {
                  "parentName": "Arts & Entertainment",
                  "name": "Art & Architecture",
                  "parentId": "9007",
                  "url": "https://itunes.apple.com/us/genre/id10002"
                }
              },
              {
                "id": "38",
                "type": "genres",
                "href": "/v1/catalog/us/genres/38?l=en-US",
                "attributes": {
                  "name": "Books",
                  "url": "https://itunes.apple.com/us/genre/id38"
                }
              }
            ]
          }
        }
      }
  ]
}

```

## Topics

### Responses

object BooksResponse

A response that contains the resource objects for the request.

object UnauthorizedResponse

A response that indicates an incorrect authorization header.

object ErrorsResponse

The collection of errors that occurred while processing the request.

## See Also

### App and book metadata

Get Metadata for Your Apps

Fetch metadata for your apps by using their identifiers.

Get Metadata for Your Books

Fetch metadata for your books by using their identifiers.

Get Metadata for a Catalog App

Fetch metadata for an app from the catalog by using its identifier.

Get Metadata for Multiple Catalog Apps

Fetch metadata for apps from the catalog by using their identifiers.

Get Metadata for Multiple Catalog Books

Fetch metadata for books from the catalog by using their identifiers.

Get Catalog Search Results

Fetch metadata for apps and books from the catalog by using a search term.

