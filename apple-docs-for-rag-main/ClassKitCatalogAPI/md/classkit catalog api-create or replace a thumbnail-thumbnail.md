

- ClassKit Catalog API
-  Create or Replace a Thumbnail 

Web Service Endpoint

# Create or Replace a Thumbnail

Store an image that represents one of your app’s assignable activities.

ClassKit 1.0+

## URL

``` source
POST https://classkit-catalog.apple.com/v1/thumbnails
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

The thumbnail identifier for the thumbnail to upload. Format this value as a URL-encoded string.

## Response Codes

` 201 ``Created`

`Created`

The request succeeded.

` 202 ``Accepted`

`Accepted`

The API accepted, but hasn’t completed the request. To ask for a status update later, see Get Status.

` 400 ``Bad Request`

`Bad Request`

The request contained an error.

` 403 ``Forbidden`

`Forbidden`

The request wasn’t authorized.

## Discussion

You can associate a thumbnail image with one or more contexts. Create an association by matching the `thumbnailId` value that you provide as a query parameter to this call with the `thumbnailId` field of a Context.Data object that you upload with a call to Create or Replace Contexts. Upload the context that references a thumbnail before uploading the thumbnail.

Provide the thumbnail image as binary data in the request body. For example, after obtaining a web token, as Authenticating Calls to the ClassKit Catalog API describes, you could use the following `curl` command to upload the image in the file `catalog.png`:

```
% curl --request POST \
       --url 'https://classkit-catalog.apple.com/v1/thumbnails?thumbnailId=catalog.png&environment=production' \
       --header 'authorization: Bearer ' \
       --header 'content-type: image/png' \
       --data-binary '@catalog.png'
```

Follow the same guidelines for creating thumbnails as you follow when working with the ClassKit API in your app. In particular, provide images that are at least 80 x 80 pixels, and no larger than 330 x 330 pixels. The system ignores thumbnails that are too small, and scales down thumbnails that are too large. Use a thumbnail with the maximum dimensions to produce the best result across devices.

If you delete every context that references a thumbnail, the system automatically deletes the thumbnail image as well.

## See Also

### Uploading Thumbnails

Get a Thumbnail

Fetch the image for one of your app’s assignable activities.

Delete a Thumbnail

Remove one of the images for your app’s assignable activities.

