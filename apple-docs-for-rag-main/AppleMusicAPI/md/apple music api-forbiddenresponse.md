

- Apple Music API
-  ForbiddenResponse 

Object

# ForbiddenResponse

A response object indicating that the request wasn’t accepted due to an issue with the authentication.

Apple Music 1.0+

``` source
object ForbiddenResponse
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

object ErrorsResponse

A response object indicating that an error occurred while processing the request.

object UnauthorizedResponse

A response object indicating that the request’s authorization is missing or invalid.

object ResourceCollectionResponse

A response object composed of resource objects for the request.

