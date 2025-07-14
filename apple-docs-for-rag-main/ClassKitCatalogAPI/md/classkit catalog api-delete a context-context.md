

- ClassKit Catalog API
-  Delete a Context 

Web Service Endpoint

# Delete a Context

Remove information that you previously stored about your app’s assignable activities.

ClassKit 1.0+

## URL

``` source
DELETE https://classkit-catalog.apple.com/v1/contexts
```

## Query Parameters

`environment`

`string`

 (Required) 

The development or production environment to use for this access. For details, see Testing Your ClassKit Catalog Implementation.

Possible Values: `development, production`

`identifierPath`

`string`

 (Required) 

The identifier path for the context to delete. Format this value as a URL-encoded JSON array of strings.

`locale`

`string`

 (Required) 

The locale of the context to delete. Use one of the identifiers supported by the Locale structure. It must match a locale that your app supports.

## Response Codes

` 202 ``Accepted`

`Accepted`

The API accepted but hasn’t completed the request. To ask for a status update later, see Get Status.

` 204 ``No Content`

`No Content`

The request succeeded.

` 400 ``Bad Request`

`Bad Request`

The request contained an error.

` 403 ``Forbidden`

`Forbidden`

The request wasn’t authorized.

## Discussion

You can’t delete a context that has child contexts. Delete any child contexts before trying to delete their parent.

### Example

- Request
- Response

```
https://classkit-catalog.apple.com/v1/contexts?environment=development&identifierPath=%5B%22com.apple.www.Quizzer%22%2C%22Quiz%20Catalog%22%5D&locale=en-us
```

```
```

## See Also

### Declaring Contexts

Preparing Context Data

Adjust how you manage context data when working with the web API.

Create or Replace Contexts

Store information about the assignable content that your educational app provides.

Get a Context

Fetch information that you previously stored about your app’s assignable activities.

object Context

An area of your app that represents an assignable task, like a quiz or a chapter.

object ContextsRequest

A request that you make when modifying context information.

object ContextsResponse

The response you receive after modifying context information.

