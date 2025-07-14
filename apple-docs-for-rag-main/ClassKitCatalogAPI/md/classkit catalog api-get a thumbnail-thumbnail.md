

- ClassKit Catalog API
-  Get a Thumbnail 

Web Service Endpoint

# Get a Thumbnail

Fetch the image for one of your app’s assignable activities.

ClassKit 1.0+

## URL

``` source
GET https://classkit-catalog.apple.com/v1/thumbnails
```

## Query Parameters

`environment`

`string`

 (Required) 

The development or production environment to use for this access. For details, see Testing Your ClassKit Catalog Implementation.

Possible Values: `development, production`

`thumbnailId`

`string`

 (Required) 

The thumbnail identifier for the thumbnail to retrieve. Format this value as a URL-encoded string.

## Response Codes

` 200 ``OK`

`OK`

The request succeeded.

` 202 ``Accepted`

`Accepted`

The API accepted but hasn’t completed the request. To ask for a status update later, see Get Status.

` 400 ``Bad Request`

`Bad Request`

The request contained an error.

` 403 ``Forbidden`

`Forbidden`

The request wasn’t authorized.

## See Also

### Uploading Thumbnails

Create or Replace a Thumbnail

Store an image that represents one of your app’s assignable activities.

Delete a Thumbnail

Remove one of the images for your app’s assignable activities.

