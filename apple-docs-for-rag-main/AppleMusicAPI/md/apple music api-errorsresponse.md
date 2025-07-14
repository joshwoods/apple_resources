

- Apple Music API
-  ErrorsResponse 

Object

# ErrorsResponse

A response object indicating that an error occurred while processing the request.

Apple Music 1.0+

``` source
object ErrorsResponse
```

## Properties

`errors`

`[`Error`]`

 (Required) 

The collection of errors that occurred while processing the request.

## See Also

### Related Objects

object EmptyBodyResponse

A response object that contains no content.

object UnauthorizedResponse

A response object indicating that the request’s authorization is missing or invalid.

object ForbiddenResponse

A response object indicating that the request wasn’t accepted due to an issue with the authentication.

object ResourceCollectionResponse

A response object composed of resource objects for the request.

