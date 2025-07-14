

- Apple Music API
-  Error 

Object

# Error

Information about an error that occurred while processing a request.

Apple Music 1.0+

``` source
object Error
```

## Properties

`code`

`string`

 (Required) 

The code for this error. For possible values, see HTTP Status Codes.

`detail`

`string`

A long, possibly localized, description of the problem.

`id`

`string`

 (Required) 

A unique identifier for this occurrence of the error.

`source`

Error.Source

An object containing references to the source of the error. For possible members, see `Source` object.

`status`

`string`

 (Required) 

The HTTP status code for this problem.

`title`

`string`

 (Required) 

A short, possibly localized, description of the problem.

## Mentioned in 

HTTP Status Codes

Handling Requests and Responses

## Discussion

If a request is unsuccessful, the `errors` in the response may contain an Error object for each problem that occurred.

## Topics

### Related Objects

object Error.Source

The Source object represents the source of an error.

## See Also

### Handling Errors

HTTP Status Codes

Reference error codes returned by the Apple Music API.

