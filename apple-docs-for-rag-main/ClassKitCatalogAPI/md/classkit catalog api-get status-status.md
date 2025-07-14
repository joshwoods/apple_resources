

- ClassKit Catalog API
-  Get Status 

Web Service Endpoint

# Get Status

Fetch the status of an operation that you initiated earlier.

ClassKit 1.0+

## URL

``` source
GET https://classkit-catalog.apple.com/v1/status/{statusId}
```

## Path Parameters

`statusId`

`string`

 (Required) 

The identifier of the operation for which you want to retrieve the status.

## Response Codes

` 200 ``OK`

Status

`OK`

The request succeeded.

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

The request contained an error.

` 403 ``Forbidden`

`Forbidden`

The request wasn’t authorized.

## Discussion

If the system can’t immediately complete a request, the ClassKit Catalog API may acknowledge that it received the request and respond with a HTTP response containing the status code `202 ACCEPTED`. In this case, the response contains a header with the name “Location”. The corresponding value is a URL that points to the Get Status endpoint, including a `statusId` as the last path parameter. The header item might look like this:

```
```

Use this `statusID` to ask the server for a status update at a later time.

### Example

- Request
- Response

```
https://classkit-catalog.apple.com/v1/status/KGW7S5VLDDOQSYSE7DKGYBGXUU 
```

```
{
  "statusId": "KGW7S5VLDDOQSYSE7DKGYBGXUU",
  "teamId": "2X6UPAGN5A",
  "state": "error",
  "statusCode": "400",
  "error": {
    "id": "KGW7S5VLDDOQSYSE7DKGYBGXUU",
    "code": "THUMBNAIL_NOT_REFERENCED",
    "message": "The thumbnail with 'thumbnailId': unreferenced_image.png is not referenced by any context."
  },
  "location": "classkit-catalog.apple.com/v1/status/KGW7S5VLDDOQSYSE7DKGYBGXUU"
}

```

## See Also

### Retrieving Status

object Status

The state of a request that the API previously accepted, but didn’t complete right away.

